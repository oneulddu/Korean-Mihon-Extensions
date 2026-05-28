# Xtoon Mihon Extension Repo

Xtoon Mihon/Tachiyomi 확장 배포 전용 저장소입니다.

## Mihon 저장소 추가 URL

Keiyoushi 배포 레포처럼 `repo` 브랜치를 배포 브랜치로 사용합니다.

```text
https://raw.githubusercontent.com/oneulddu/Xtoon-Mihon-Extension/repo/index.min.json
```

기존 `main` 주소도 현재는 같은 파일을 가리키도록 유지합니다.

```text
https://raw.githubusercontent.com/oneulddu/Xtoon-Mihon-Extension/main/index.min.json
```

## 배포 파일

- APK: `apk/tachiyomi-ko.xtoon-v1.4.4-release.apk`
- 아이콘: `icon/eu.kanade.tachiyomi.extension.ko.xtoon.png`
- 구형 저장소 목록: `index.min.json`
- 신형 저장소 목록: `index.json`
- 저장소 정보: `repo.json`

## 소스 코드

확장 소스와 Gradle 빌드 환경은 별도 레포로 분리했습니다.

```text
https://github.com/oneulddu/Korean-Mihon-Extensions-Source
```

## 현재 배포 버전

```text
version: 1.4.4
versionCode: 4
baseUrl: https://t3.xtoon365.com
```

## 서명 정보

현재 APK는 로컬 release 키로 서명되어 있습니다.

```text
SHA-256: 62aaff9a192e8d3e462b352a4b435bcacc38c2390aa9c0dbf9c863942401adf0
```

`signingkey.jks`와 `signing.env`는 Git에 올리지 않고 별도로 보관합니다.

## GitHub Actions

자동 빌드/자동 인덱스 갱신은 소스 레포에서 관리합니다.

```text
https://github.com/oneulddu/Korean-Mihon-Extensions-Source/actions/workflows/build_xtoon_release.yml
```

해당 workflow가 Xtoon APK를 빌드하고 이 레포의 `repo` 브랜치에 APK, 아이콘, `index.json`, `index.min.json`, `repo.json`을 갱신합니다.

## 주의

로그인, 결제, 성인 인증, 캡차, 차단 우회, DRM 우회 목적의 구현은 포함하지 않습니다.
