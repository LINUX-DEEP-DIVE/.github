# `.github` — org-wide defaults for LINUX DEEP DIVE

이 레포는 `LINUX-DEEP-DIVE` org의 **공용 커뮤니티 헬스 파일**을 담습니다.
여기 있는 이슈/PR 템플릿은 org 안의 **모든 레포에 자동 상속**됩니다. (각 레포에
자체 템플릿이 있으면 그 레포에서는 자체 것이 우선합니다.)

## 담고 있는 것

```
.github/
  ISSUE_TEMPLATE/
    config.yml          # 빈 이슈 비활성화 (blank_issues_enabled: false)
    bug-report.md       # 버그 리포트 (Go / Linux 커널 환경 항목)
    feature-request.md  # Enhancement Request
    common-issue.md     # Common Issue
  PULL_REQUEST_TEMPLATE.md
profile/
  README.md             # org 랜딩 페이지(github.com/LINUX-DEEP-DIVE)에 표시
```

> 출처: [yorkie-team/yorkie](https://github.com/yorkie-team/yorkie) 방식을 차용.

## 상속 규칙 (중요)

GitHub의 org `.github` 레포로 **상속되는 것**: 이슈 템플릿, PR 템플릿,
`CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `profile/README.md` 등.

**상속되지 않는 것** (레포마다 따로 둬야 함): `dependabot.yml`,
GitHub Actions 워크플로(`.github/workflows/`), 그리고 CodeRabbit 설정
(`.coderabbit.yaml`).

## CodeRabbit (AI PR 리뷰) 설정 — 무료(public 레포)

**설정 파일은 필요 없고**, org에 GitHub App 한 번만 설치하면 기본값으로 동작합니다.

1. https://coderabbit.ai → **Login with GitHub**
2. `LINUX-DEEP-DIVE` org에 App 설치. public 레포는 **CodeRabbit Pro 무료**.
3. 적용할 레포 선택(또는 all repositories). 끝 — 이후 열리는 PR마다 자동 리뷰.
4. (선택) 리뷰 톤·언어 등을 바꾸고 싶으면 해당 **코드 레포**(이 `.github` 레포가
   아니라)에 `.coderabbit.yaml`을 추가. org 전체 기본값은 CodeRabbit 대시보드에서.

