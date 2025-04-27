# ytstampy-daliah

## 준비물

[uv](https://docs.astral.sh/uv/getting-started/installation/)

```sh
winget install astral-sh.uv                     # windows
curl -LsSf https://astral.sh/uv/install.sh | sh # mac, linux
brew install uv                                 # mac, linux
```

## 프로젝트 준비

1. 프로젝트 받기

```sh
git clone https://github.com/utawakuworker/ytstampy-daliah
cd ytstampy-daliah
```

2. 파이썬 환경 및 라이브러리 설치

```sh
uv sync
```

## 빌드

### flet

```sh
uv run flet build windows
uv run flet build macos
uv run flet build linux
```

## 개발

```sh
uv run poe dev
```

## 스크립트

| 스크립트 | 동작 |
| --------------- | ---------------------- |
| `uv run flet` | `flet` cli 실행 |
| `uv run poe dev` | 개발용 |
| `uv run poe format` | 프로젝트 전체 포맷 |
| `uv run poe lint` | 프로젝트 전체 린트 |
| `uv sync` | 프로젝트 환경 싱크 |
| `uv add XYZ` | `XYZ` 패키지 추가 |
| `uv add --dev XYZ` | 개발 환경용 `XYZ` 패키지 추가 |
| `uv -h` | `uv` 헬프 메시지 |
