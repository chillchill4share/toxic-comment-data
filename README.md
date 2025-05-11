Tiếng Việt
Dự án này chứa các file CSV dùng để phân loại văn bản tiếng Việt thành độc hại (1) hoặc không độc hại (0). Các file bao gồm:

1. chill_train.csv: Dữ liệu huấn luyện, chứa cột free_text (văn bản) và label_id (nhãn: 0 hoặc 1). Dữ liệu bao gồm các bình luận, trạng thái mạng xã hội, hoặc văn bản ngắn khác bằng tiếng Việt.
2. chill_dev.csv: Dữ liệu xác thực, cấu trúc tương tự chill_train.csv, dùng để đánh giá mô hình trong quá trình huấn luyện.
3. chill_test.csv: Dữ liệu kiểm tra, cấu trúc tương tự chill_train.csv, dùng để đánh giá hiệu suất cuối cùng của mô hình.

Lưu ý:

- Văn bản trong các file chứa tiếng Việt có dấu, không dấu, tiếng lóng, emoji, và đôi khi có ngôn từ thô tục.
- Nhãn 0 biểu thị văn bản không độc hại (bình thường, tích cực), nhãn 1 biểu thị văn bản độc hại (xúc phạm, thô tục, tiêu cực).
- Dữ liệu phản ánh ngôn ngữ thực tế trên mạng xã hội, cần được tiền xử lý (làm sạch, chuẩn hóa) trước khi huấn luyện mô hình.

English
This project contains CSV files for classifying Vietnamese text as toxic (1) or non-toxic (0). The files include:

1. chill_train.csv: Training data, with columns free_text (text) and label_id (labels: 0 or 1). The data consists of comments, social media posts, or other short texts in Vietnamese.
2. chill_dev.csv: Validation data, with the same structure as chill_train.csv, used to evaluate the model during training.
3. chill_test.csv: Test data, with the same structure as chill_train.csv, used to assess the final performance of the model.

Note:

- The text in the files includes Vietnamese with and without diacritics, slang, emojis, and sometimes vulgar language.
- Label 0 indicates non-toxic text (normal, positive), while label 1 indicates toxic text (offensive, vulgar, negative).
- The data reflects real-world social media language and requires preprocessing (cleaning, normalization) before model training.