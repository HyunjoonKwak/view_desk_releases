# View Desk — 릴리스

맥에 있는 사진·영상과 OTT를 한 곳에서 여는 개인용 앱 **View Desk**의 배포 파일만 두는 저장소입니다.
소스 코드는 여기에 없습니다.

## 받기

[Releases](../../releases/latest)에서 `View Desk-<버전>-arm64.dmg`를 받습니다.

- Apple Silicon 맥 전용(arm64), macOS 13 이상
- 0.8.3부터는 앱의 설정 › 업데이트에서 새 버전을 바로 받습니다

## 처음 설치할 때

이 앱은 Apple 공증을 받지 않았습니다. 브라우저로 받은 파일은 macOS가 실행을 막으므로, dmg를 열어
`View Desk.app`을 응용 프로그램 폴더로 옮긴 뒤 터미널에서 한 번 실행합니다.

```bash
xattr -dr com.apple.quarantine "/Applications/View Desk.app"
```

터미널을 쓰지 않으려면 앱을 한 번 실행해 차단 창을 띄운 뒤, 시스템 설정 › 개인정보 보호 및 보안 맨 아래의
«그래도 열기»를 누릅니다.

## 파일 확인

각 릴리스의 `SHA256SUMS`에 dmg와 zip의 SHA-256이 들어 있습니다.

```bash
shasum -a 256 "View Desk-<버전>-arm64.dmg"
```
