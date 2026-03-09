# git_workflow_gitlabflow_practice

_**Giả sử dự án:**_

Một công ty phát triển ứng dụng web lớn và triển khai(deploy) theo nhiều môi trường:

development(phát triển)
staging(dàn dựng)
production(sản xuất)

Nhóm quyết định sử dụng GitLab Flow.

_**Các branch**_
main → code mới nhất
production → code đang chạy thật
staging → môi trường test
feature/* → tính năng

_**Cấu trúc**_
```
main
├─ feature/login
├─ feature/payment
```
_**Sau khi hoàn thành:**_
feature → merge → main
_**Sau đó deploy qua các môi trường:**_
main → staging → production

_**Workflow**_
Developer làm việc trên feature branch.
feature → main
_**Sau đó deploy:**_
main → staging → production

_**Ví dụ**_
```
main
↓
staging
↓
production
```
Nếu staging test OK → merge sang production.

_**Mục đích repo minh họa**_
- feature development
- môi trường staging
- deploy production
