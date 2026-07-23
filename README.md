# NEXTCORE SOLUTIONS

> Real fixes for the small, maddening problems that quietly eat your dev machine, your CI bill, and your AI agent's sanity.
> Những lời giải cho các vấn đề nhỏ mà dai dẳng — thứ âm thầm ngốn tài nguyên máy, hoá đơn CI, và làm "kẹt" con AI agent của bạn.

Most of these look trivial until you hit them at 2 AM. They're the kind of thing an AI coding agent (Claude, Cursor, …) — or you — runs into, shrugs at, and works around badly. Here are the clean fixes, battle-tested in production.

Phần lớn trông tầm thường cho tới lúc bạn dính nó lúc 2 giờ sáng. Đây là kiểu lỗi mà một AI agent (Claude, Cursor…) — hoặc chính bạn — gặp rồi né tạm bợ. Dưới đây là cách sửa gọn, đã kiểm chứng thực tế.

---

## Solutions / Danh mục

| # | Problem | Fix |
|---|---------|-----|
| 01 | Node.js processes pile up on Windows and lag the whole machine (MCP servers, dev tasks that never die) | [orphan-node-reaper](./orphan-node-reaper/) |
| 02 | Chrome MCP "lost connection" / "browser already running" — agent gives up and asks you to check | [chrome-mcp-resilience](./chrome-mcp-resilience/) |

More coming. Each folder is self-contained: the *why*, the *fix*, and a drop-in script.

Mỗi thư mục tự đủ: *vì sao*, *cách sửa*, và script dùng ngay.

---

## Philosophy / Tinh thần

- **Root cause, not workaround.** We explain *why* it happens before handing you the fix.
- **Safe by default.** Scripts only touch what they prove is orphaned/broken — never your live work.
- **Copy-paste ready.** No framework, no install ceremony.

Tìm gốc rễ, không chắp vá · An toàn mặc định (chỉ đụng thứ đã chứng minh là mồ côi/hỏng) · Dán-là-chạy.

---

## Contributing / Đóng góp

Hit a gotcha we haven't covered? Open an issue with the symptom + your environment. If it's reproducible and the fix is clean, it goes in.

Gặp lỗi chưa có ở đây? Mở issue kèm triệu chứng + môi trường. Tái hiện được + fix gọn thì lên repo.

## License

MIT — use freely, no attribution required (but a star is nice).
