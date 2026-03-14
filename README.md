# linkhub-cron-jobs

linkhub 프로젝트의 정기 DB 작업을 관리하는 레포입니다.

## 워크플로우

### sync-db
- **주기**: 매일 오전 6시 KST
- **내용**: 운영 DB(`links`) → 스테이지 DB(`links_staging`) 데이터 동기화

## 시크릿 설정

GitHub 레포 Settings → Secrets and variables → Actions에 다음을 등록합니다.

| 이름 | 값 |
|------|-----|
| `DB_URL` | Supabase 프로젝트의 DB 연결 URL (비밀번호 포함) |
