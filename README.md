# nutriplate
“PTIT Image Processing BTL – single tray nutrition analysis
## Mục tiêu
Phân tích 01 ảnh khay 4 ngăn, hiển thị ảnh căn chỉnh,
mask/overlay và tính kcal, protein, fat, carb từ tên món,
khối lượng (g) do người dùng nhập.
Không phân tích sau ăn; không tự suy ra gram từ 01 ảnh RGB.

## Môi trường
- Python 3.11 (môi trường đề xuất, phải test thực tế)
- Windows/Linux/macOS; webcam KHÔNG bắt buộc

## Cài đặt
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt

## Chạy ứng dụng
streamlit run app.py

## Kiểm thử
python -m pytest -q

## Dữ liệu & mô-đun
- data/nutrition_reference.csv: bảng dinh dưỡng/100 g có nguồn
- config/tray_layout_v1.json: bốn ROI C1–C4
- src/: các module M1–M6
- runs/<run_id>/: kết quả chạy cục bộ, không commit

## Quy trình đóng góp
Tạo nhánh feat/fix/docs/test/chore → commit → push → PR
vào main → reviewer khác kiểm tra → merge.
Xem docs/Git_Repo_README_Convention.docx.

## Thành viên & giới hạn
TV1 M1/M2 · TV2 M3 · TV3 M4/M5 · TV4 M6/tích hợp
Chỉ demo một kiểu khay, 3–4 món quen thuộc.
