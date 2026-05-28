# Xtoon Mihon Extension Repo

Xtoon Mihon/Tachiyomi 확장 배포 전용 저장소입니다.

## Mihon 저장소 추가 URL

Mihon의 확장 저장소에 아래 URL을 추가하면 됩니다.

```text
https://raw.githubusercontent.com/oneulddu/Xtoon-Mihon-Extension/main/index.min.json
```

## 배포 파일

- APK: `apk/tachiyomi-ko.xtoon-v1.4.4-release.apk`
- 아이콘: `icon/eu.kanade.tachiyomi.extension.ko.xtoon.png`
- 저장소 정보: `repo.json`
- 확장 목록: `index.json`, `index.min.json`

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

## 주의

로그인, 결제, 성인 인증, 캡차, 차단 우회, DRM 우회 목적의 구현은 포함하지 않습니다.
