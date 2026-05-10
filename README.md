# My Assistant Testing

Repository thử nghiệm cho tích hợp Claude Code với GitHub Actions.

## Tổng quan

Repository này minh họa việc tích hợp Claude Code với GitHub Actions sử dụng 9Router làm lớp proxy API.

## Tính năng

- Tích hợp GitHub Issues với Claude Code
- Hỗ trợ Pull Request
- Tự động review và triển khai code

## Cài đặt

Repository này sử dụng 9Router làm proxy cho Anthropic API:

- 9Router chạy trên cổng `20128`
- Claude Code kết nối qua `http://localhost:20128/v1`

## Cách sử dụng

### Làm việc với Issues

1. Tạo một issue hoặc bình luận trên issue đã có
2. Tag `@claude` trong bình luận của bạn
3. Claude Code sẽ phân tích và trả lời yêu cầu của bạn

### Làm việc với Pull Requests

1. Mở một pull request
2. Thêm review hoặc bình luận với `@claude`
3. Claude Code sẽ review và đưa ra phản hồi

## Workflow

Workflow của Claude Code được định nghĩa trong `.github/workflows/claude.yml` và xử lý:
- Bình luận trên issues
- Review PR
- Các tác vụ triển khai code

## Giấy phép

MIT
