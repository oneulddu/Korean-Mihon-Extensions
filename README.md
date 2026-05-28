# Korean Mihon Extensions Repo

한국어 Mihon/Tachiyomi 확장 배포 전용 저장소입니다.

## Mihon 저장소 추가 URL

Keiyoushi 배포 레포처럼 `repo` 브랜치를 배포 브랜치로 사용합니다.

```text
https://raw.githubusercontent.com/oneulddu/Korean-Mihon-Extensions/repo/index.min.json
```

## 배포 파일

- `11toon`: `apk/tachiyomi-ko.toon11-v1.4.2-release.apk`
- `BlackToon`: `apk/tachiyomi-ko.blacktoon-v1.4.1-release.apk`
- `Manatoki`: `apk/tachiyomi-ko.manatoki-v1.4.1-release.apk`
- `Naver Comic`: `apk/tachiyomi-ko.navercomic-v1.4.7-release.apk`
- `NTK`: `apk/tachiyomi-ko.ntk-v1.4.5-release.apk`
- `Toonkor`: `apk/tachiyomi-ko.toonkor-v1.4.6-release.apk`
- `Wolf.com`: `apk/tachiyomi-ko.wolfdotcom-v1.4.3-release.apk`
- `Xtoon`: `apk/tachiyomi-ko.xtoon-v1.4.4-release.apk`

- 구형 저장소 목록: `index.min.json`
- 신형 저장소 목록: `index.json`
- 저장소 정보: `repo.json`

## 소스 코드

확장 소스와 Gradle 빌드 환경은 별도 레포로 분리했습니다.

```text
https://github.com/oneulddu/Korean-Mihon-Extensions-Source
```

## 서명 정보

현재 APK는 release 키로 서명되어 있습니다.

```text
SHA-256: b25af02d178fad20ebe739e59336f2ae5e307dcd1375418278e752dba03497cb
```

`signingkey.jks`와 `signing.env`는 Git에 올리지 않고 별도로 보관합니다.

## GitHub Actions

자동 빌드/자동 인덱스 갱신은 소스 레포에서 관리합니다.

```text
https://github.com/oneulddu/Korean-Mihon-Extensions-Source/actions/workflows/build_extensions_release.yml
```

해당 workflow가 한국어 확장 APK를 빌드하고 이 레포의 `repo` 브랜치에 APK, 아이콘, `index.json`, `index.min.json`, `repo.json`을 갱신합니다.

## 주의

로그인, 결제, 성인 인증, 캡차, 차단 우회, DRM 우회 목적의 구현은 포함하지 않습니다.
