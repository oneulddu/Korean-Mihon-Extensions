<div align="center">

# 📚 Korean Mihon Extensions

**한국어 만화·웹툰 소스를 위한 [Mihon](https://mihon.app) / Tachiyomi 확장 배포 저장소**

[![Mihon 저장소 추가](https://img.shields.io/badge/Mihon-저장소_추가-2979FF?style=for-the-badge&logo=android&logoColor=white)](https://intradeus.github.io/http-protocol-redirector?r=tachiyomi://add-repo?url=https://raw.githubusercontent.com/oneulddu/Korean-Mihon-Extensions/repo/index.min.json)
[![Source](https://img.shields.io/badge/Source-소스_코드-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/oneulddu/Korean-Mihon-Extensions-Source)
![Language](https://img.shields.io/badge/Language-한국어-success?style=for-the-badge)

</div>

---

## ✨ 소개

이 저장소는 한국어 만화·웹툰 사이트를 위한 Mihon / Tachiyomi 확장(APK)을 모아 배포하는 **배포 전용 저장소**입니다.
[Keiyoushi](https://github.com/keiyoushi/extensions) 배포 레포와 동일하게 `repo` 브랜치를 배포 브랜치로 사용합니다.

---

## 🚀 저장소 추가하기

Mihon 앱에서 아래 URL을 확장 저장소로 추가하세요.

```text
https://raw.githubusercontent.com/oneulddu/Korean-Mihon-Extensions/repo/index.min.json
```

> **빠른 추가** — 안드로이드 기기에서 아래 배지를 누르면 Mihon에 바로 저장소가 추가됩니다.
>
> [![Mihon에 바로 추가](https://img.shields.io/badge/Mihon에_바로_추가-2979FF?style=flat-square&logo=android&logoColor=white)](https://intradeus.github.io/http-protocol-redirector?r=tachiyomi://add-repo?url=https://raw.githubusercontent.com/oneulddu/Korean-Mihon-Extensions/repo/index.min.json)

**수동 추가 방법**

1. Mihon → **설정 → 브라우즈 → 확장 저장소**
2. 위 URL을 입력하고 추가
3. **브라우즈 → 확장** 탭에서 원하는 확장을 설치

---

## 📦 제공 확장

<!-- 아래 표는 소스 레포의 scripts/update_repo.py가 index.json 기준으로 자동 갱신합니다. 직접 수정하지 마세요. -->
<!-- extensions:start -->
| 확장 | 버전 | 사이트 | 패키지 |
| :--- | :--: | :--- | :--- |
| 11toon | `1.4.3` | [www.11toon.com](https://www.11toon.com) | `…ko.toon11` |
| BlackToon | `1.4.7` | [blacktoon416.com](https://blacktoon416.com) | `…ko.blacktoon` |
| Jjaptoon | `1.4.6` | [www.jjaptoon003.com](https://www.jjaptoon003.com) | `…ko.jjaptoon` |
| Manatoki | `1.4.1` | [manatoki552.net](https://manatoki552.net) | `…ko.manatoki` |
| Naver Comic | `1.4.7` | [comic.naver.com](https://comic.naver.com) | `…ko.navercomic` |
| NTK | `1.4.12` | [sbxh9.com/manhwa](https://sbxh9.com/manhwa) | `…ko.ntk` |
| RawDEX | `1.4.54` | [rawdex.net](https://rawdex.net) | `…ko.rawdex` |
| Toonkor | `1.4.7` | [tkor136.com](https://tkor136.com) | `…ko.toonkor` |
| Wolf.com | `1.4.6` | [wfwf421.com](https://wfwf421.com) | `…ko.wolfdotcom` |
| Xtoon | `1.4.4` | [t3.xtoon365.com](https://t3.xtoon365.com) | `…ko.xtoon` |
<!-- extensions:end -->

> 위 표는 소스 레포의 빌드 워크플로가 [`index.json`](index.json)을 기준으로 자동 갱신합니다.

---

## 🗂️ 저장소 구조

| 경로 | 설명 |
| :--- | :--- |
| `apk/` | 배포용 확장 APK |
| `icon/` | 확장 아이콘 |
| `index.json` | 신형 저장소 인덱스 (사람이 읽기 좋은 형식) |
| `index.min.json` | 구형 / Mihon용 압축 인덱스 |
| `repo.json` | 저장소 메타데이터 (이름·웹사이트·서명 지문) |
| `index.html` | 저장소 안내 페이지 |

---

## 🔐 서명 정보

모든 APK는 동일한 release 키로 서명되어 있습니다.

```text
SHA-256: b25af02d178fad20ebe739e59336f2ae5e307dcd1375418278e752dba03497cb
```

> `signingkey.jks`와 `signing.env`는 Git에 포함하지 않고 별도로 안전하게 보관합니다.

---

## 🛠️ 소스 코드 & 자동 빌드

확장 소스 코드와 Gradle 빌드 환경은 별도 레포에서 관리합니다.

```text
https://github.com/oneulddu/Korean-Mihon-Extensions-Source
```

[GitHub Actions 워크플로](https://github.com/oneulddu/Korean-Mihon-Extensions-Source/actions/workflows/build_extensions_release.yml)가
확장 APK를 빌드한 뒤, 이 레포의 `repo` 브랜치에 APK·아이콘·`index.json`·`index.min.json`·`repo.json`과
위 확장 표(`README.md`)를 자동으로 갱신합니다.

---

## ⚠️ 주의

- 본 확장은 **공개된 한국어 만화·웹툰 사이트의 콘텐츠를 Mihon에서 열람하기 위한 용도**입니다.
- 로그인, 결제, 성인 인증, 캡차, 차단 우회, DRM 우회 목적의 구현은 **포함하지 않습니다.**
- 콘텐츠 저작권은 각 원저작자 및 해당 사이트에 있으며, 이용에 대한 책임은 사용자 본인에게 있습니다.

---

## 📄 라이선스

이 저장소는 [Apache License 2.0](LICENSE)을 따릅니다.

<div align="center">

---

Made with ❤️ for the Korean Mihon community

</div>
