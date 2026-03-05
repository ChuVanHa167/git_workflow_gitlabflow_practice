# git_workflow_gitlabflow_practice

Giả sử dự án
Một công ty phát triển ứng dụng web lớn và triển khai(deploy) theo nhiều môi trường:
(phát triển)development
(dàn dựng)staging
(sản xuất)production
Nhóm quyết định sử dụng GitLab Flow.

Các branch
main → code mới nhất
production → code đang chạy thật
staging → môi trường test
feature/* → tính năng

Cấu trúc
main
├─ feature/login
├─ feature/payment
Sau khi hoàn thành:
feature → merge → main
Sau đó deploy qua các môi trường:
main → staging → production

Workflow
Developer làm việc trên feature branch.
feature → main
Sau đó deploy:
main → staging → production

Ví dụ
main
↓
staging
↓
production
Nếu staging test OK → merge sang production.

Mục đích repo
Repo này minh họa:
feature development

môi trường staging

deploy production
