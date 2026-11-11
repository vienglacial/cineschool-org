# CineSchool.ORG Studio

Bản cài đặt dành cho học viên CineSchool.ORG, có cho **Windows** và **Mac**.

## Tải về

Vào mục **[Releases](../../releases/latest)** và tải đúng file cho máy của bạn (`x.y.z` là số phiên bản):

| Máy của bạn | File cần tải |
|---|---|
| Windows 10 / 11 (64-bit) | `CineSchool-Setup-x.y.z.exe` |
| Mac chip Apple (M1, M2, M3, M4…) | `CineSchool-x.y.z-mac-arm64.dmg` |
| Mac chip Intel | `CineSchool-x.y.z-mac-x64.dmg` |

Chưa biết Mac của mình dùng chip gì: bấm biểu tượng quả táo ở góc trên bên trái → **About This Mac** (Giới thiệu về máy Mac này), xem dòng **Chip** hoặc **Processor**.

## Cài trên Windows

Mở file `.exe` vừa tải rồi làm theo các bước. App cài cho người dùng hiện tại, không cần quyền admin.

Cài xong app **tự cập nhật** mỗi khi có bản mới, không cần tải lại.

## Cài trên Mac

Cần macOS 11 (Big Sur) trở lên.

1. Mở file `.dmg` vừa tải, kéo biểu tượng **CineSchool.ORG** sang thư mục **Applications**.
2. App chưa có chữ ký của Apple, nên lần đầu mở Mac sẽ chặn và báo app "bị hỏng" (is damaged) hoặc "không thể xác minh". App không hỏng: bấm **Cancel** (Huỷ), đừng bấm Move to Trash, rồi làm tiếp:
   - Mở ứng dụng **Terminal** (bấm `⌘ + Space`, gõ `Terminal`, bấm Enter).
   - Dán dòng dưới đây vào rồi bấm Enter. Không hiện gì thêm nghĩa là đã xong.

     ```
     xattr -cr /Applications/CineSchool.ORG.app
     ```
3. Mở app như bình thường. Lần đầu lưu file, Mac hỏi quyền vào thư mục Documents: chọn **Allow** (Cho phép).

Trong file `.dmg` cũng có sẵn file hướng dẫn `Doc truoc khi cai.txt`.

### Khi có bản mới trên Mac

Trên Mac app chưa tự cài bản mới được. Khi có bản mới, app báo ở góc dưới màn hình:

1. Bấm **Tải về** để tải file `.dmg` mới.
2. Tắt app, mở file `.dmg`, kéo app sang **Applications** và chọn **Replace** (Thay thế).
3. Chạy lại lệnh `xattr -cr` ở trên rồi mở app.

Project và dữ liệu của bạn giữ nguyên.

### Khác với Windows một chút

- Phím `Ctrl` trong hướng dẫn tương ứng phím `⌘ Command` trên Mac.
- Trên canvas video: vuốt hai ngón để kéo, chụm hai ngón (hoặc giữ `⌘` rồi lăn chuột) để phóng to, thu nhỏ.

## Ghi chú

Repo này **chỉ chứa file cài đặt**, không chứa mã nguồn.
