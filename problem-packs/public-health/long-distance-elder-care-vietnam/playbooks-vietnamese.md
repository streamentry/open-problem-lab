# Kế hoạch tổng thể

> Đây là bản tiếng Việt của `playbooks.md`, được viết để phục vụ triển khai và
> thẩm định tại Việt Nam. `playbooks.md` vẫn là tài liệu chuẩn. Nếu hai bản có
> điểm không thống nhất, phải sửa bản tiếng Việt cho khớp với bản chuẩn, không
> được tự suy diễn thành một quy trình khác.

## Luận đề chiến lược

Sản phẩm cốt lõi là khả năng hỗ trợ tại chỗ đã được xác minh, không phải khả
năng quan sát từ xa. Chỉ xem xét phát triển phần mềm sau khi một dịch vụ vận
hành thủ công chứng minh được bốn điều: người cao tuổi thực sự muốn sử dụng;
nhân sự tại chỗ có thể cung cấp hỗ trợ; các tình huống cần chuyển cấp được xử lý
đến nơi đến chốn; và toàn bộ chi phí nhân công, đi lại, giám sát có nguồn chi
trả khả thi.

## Người dùng và quyết định

| Người dùng                                 | Quyết định                                                                                                              |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| Người cao tuổi                             | Chấp nhận, từ chối hoặc rút lại loại hỗ trợ nào; cho phép chia sẻ thông tin nào.                                        |
| Người thân sống xa                         | Có cần một dịch vụ hỗ trợ tại chỗ đã được xác minh hay không; gia đình tiếp tục chịu trách nhiệm ở khâu chuyển cấp nào. |
| Nhân sự hỗ trợ tại chỗ hoặc người giám sát | Yêu cầu thuộc loại thông thường, khẩn cấp hay ngoài phạm vi; đã giải quyết, đã chuyển giao hay còn tồn đọng.            |
| Đối tác cấp xã hoặc cơ sở chăm sóc ban đầu | Có đưa người cao tuổi vào quy trình đánh giá hoặc chuyển tuyến sẵn có hay không.                                        |
| Đơn vị vận hành chương trình               | Dừng, thiết kế lại, tiếp tục vận hành thủ công hay cho phép phát triển phần mềm.                                        |

## Giai đoạn 0: Xác định ranh giới dịch vụ

1. Chọn một địa bàn nhỏ, liền mạch và có thể giám sát.
2. Định nghĩa rõ “người cao tuổi”, “người thân sống xa” và khoảng thời gian phản
   hồi có ý nghĩa, nhưng không coi các ngưỡng này là chuẩn chung cho cả nước.
3. Tách biệt năm loại việc: đồng hành tinh thần; hỗ trợ hoạt động sinh hoạt hằng
   ngày; điều phối chăm sóc; chăm sóc lâm sàng; ứng cứu khẩn cấp.
4. Ghi rõ những dịch vụ nằm ngoài phạm vi.
5. Chỉ định cơ sở y tế có giấy phép và dịch vụ khẩn cấp tiếp tục chịu trách
   nhiệm chuyên môn.

Điều kiện qua giai đoạn: mỗi nhóm dịch vụ phải có một bên chịu trách nhiệm, một
trường hợp không được áp dụng và một điểm tiếp nhận chuyển cấp.

## Giai đoạn 1: Đo khoảng trống trong khả năng đáp ứng chăm sóc

Thiết kế các trường dữ liệu riêng cho:

- hoàn cảnh sống
- nguyện vọng của người cao tuổi
- nhu cầu hỗ trợ chức năng
- nguồn chăm sóc có trả phí và không trả phí hiện có
- thời gian di chuyển và khả năng có mặt thực tế của gia đình
- hàng xóm đáng tin cậy hoặc mạng lưới hỗ trợ cộng đồng
- dịch vụ sẵn có tại địa phương
- khả năng tiếp cận điện thoại và các kênh liên lạc

Không công bố quy mô thị trường khi thiếu bất kỳ trường dữ liệu then chốt nào.
Chỉ báo cáo nhóm đã xác định được và phần còn lại chưa đủ dữ liệu.

Điều kiện qua giai đoạn: một người tái lập độc lập có thể dựng lại mẫu số và xác
định đầy đủ các phần dữ liệu bị thiếu.

## Giai đoạn 2: Xác minh mạng lưới hỗ trợ tại chỗ

Với từng nhân sự hỗ trợ và từng phương án dự phòng:

1. xác minh danh tính, vai trò, đào tạo, giờ hoạt động, địa bàn phụ trách, phương
   tiện di chuyển và cơ chế giám sát
2. gọi thử hoặc kiểm tra trực tiếp đường liên hệ
3. xác định rõ việc họ được làm và không được làm
4. ghi lại quy trình chuyển giao cho chăm sóc ban đầu, công tác xã hội, gia đình
   và dịch vụ khẩn cấp
5. ghi rõ cách xử lý khi không có ai sẵn sàng tiếp nhận

Điều kiện qua giai đoạn: không một quy trình an toàn nào được kết thúc bằng một
danh sách chưa xác minh, một giả định về tình nguyện viên hoặc một số điện thoại
không có người trả lời.

## Giai đoạn 3: Thí điểm dịch vụ điều phối thủ công

Thiết kế khởi đầu được đề xuất là một thí điểm vận hành nhỏ trong sáu tuần, sử
dụng điện thoại, công cụ nhắn tin sẵn có và biểu mẫu có cấu trúc. Cỡ mẫu chỉ
phục vụ việc học quy trình, không dùng để ước tính tác động sức khỏe.

Các chức năng dịch vụ có thể thử nghiệm:

- liên lạc định kỳ sau khi đã có sự đồng thuận
- đối chiếu danh sách thuốc và lịch hẹn, tuyệt đối không kê đơn
- quan sát cơ bản về an toàn trong nhà
- trò chuyện, đồng hành và hướng dẫn tiếp cận dịch vụ
- đến tận nơi khi xuất hiện một tín hiệu phi lâm sàng đã được quy định trước
- chuyển giao cho cơ sở có giấy phép hoặc dịch vụ khẩn cấp khi tình huống vượt
  phạm vi
- gửi thông tin xác nhận kết thúc vụ việc cho người cao tuổi và người thân đã
  được cho phép nhận thông tin

Các trạng thái sự kiện bắt buộc:

```text
requested -> acknowledged -> reached -> resolved | transferred | unresolved
đã yêu cầu -> đã tiếp nhận -> đã tiếp cận trực tiếp -> đã giải quyết | đã chuyển giao | chưa giải quyết
```

Các chỉ số bắt buộc:

- số người đủ điều kiện, được tiếp cận, tham gia, từ chối và rút lui
- tỷ lệ hoàn tất các lần liên lạc theo lịch
- phân bố thời gian phản hồi và thời gian tiếp cận trực tiếp
- số vụ việc đã giải quyết, đã chuyển giao và chưa giải quyết
- số lần chuyển cấp sai hoặc không cần thiết
- sự cố về quyền riêng tư, bảo vệ an toàn, phòng ngừa xâm hại và khiếu nại
- gánh nặng đối với người cao tuổi và nhân sự hỗ trợ
- chi phí đi lại, nhân công, giám sát và liên lạc
- bằng chứng về khoản gia đình thực trả hoặc nguồn chi trả công, tách riêng khỏi
  lời bày tỏ quan tâm

Thí điểm này không được dùng để ước tính mức giảm tử vong, số ca khẩn cấp được
ngăn ngừa, số lượt nhập viện tránh được hoặc hiệu quả lâm sàng.

## Giai đoạn 4: Các phép thử bác bỏ ít tốn kém nhất

Dừng hoặc thiết kế lại trước khi viết phần mềm nếu xuất hiện một trong các tình
huống sau:

- người cao tuổi không thể tự do đồng thuận, hoặc thường xuyên rút lui vì cảm
  thấy bị xâm phạm
- không có nhân sự tại chỗ đáng tin cậy có thể tiếp cận người tham gia trong
  khoảng thời gian đã cam kết
- các vụ việc chưa giải quyết bị che giấu, đổi nhãn hoặc dồn có hệ thống vào
  ngoài giờ trực
- chi phí đi lại và giám sát vượt quá nguồn chi trả có căn cứ
- gia đình muốn được yên tâm nhưng không sẵn sàng trả cho dịch vụ con người đứng
  sau sự yên tâm đó
- dịch vụ địa phương không thể tiếp nhận các trường hợp được chuyển giao
- dịch vụ làm tăng xung đột, cưỡng ép, gian lận, bỏ bê hoặc xử lý thuốc không an
  toàn

Các ngưỡng cho quyết định tiếp tục hay dừng trong tương lai phải được đăng ký
trước với người thẩm định tại địa phương. Gói vấn đề này không tự đặt ra một tỷ
lệ chấp nhận chung cho mọi địa bàn.

## Giai đoạn 5: Điều kiện cho phép phát triển phần mềm

Chỉ được đề xuất phần mềm sau khi dịch vụ thủ công vượt qua Giai đoạn 0 đến
Giai đoạn 4. Phần mềm đầu tiên phải giảm những điểm nghẽn vận hành đã được xác
minh:

- hồ sơ đồng thuận và người đại diện
- lịch làm việc
- trạng thái sự kiện có cấu trúc
- định tuyến chuyển cấp
- nhật ký kiểm toán
- thông tin tối thiểu gửi cho gia đình trong phạm vi đã được cho phép
- rà soát các vụ việc chưa giải quyết

Không bắt đầu bằng giám sát liên tục, điểm rủi ro dự đoán, chẩn đoán tự động
hoặc cơ chế ưu tiên thiếu minh bạch.

## Đánh đổi

| Lựa chọn                      | Lợi ích                                                    | Chi phí hoặc dạng thất bại                                                            |
| ----------------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| Tăng mức giám sát             | Có thể phát hiện tín hiệu sớm hơn                          | Xâm phạm đời tư, báo động giả, suy giảm quyền tự chủ và cảnh báo không có người xử lý |
| Cam kết phản hồi nhanh hơn    | Tăng giá trị cảm nhận đối với gia đình                     | Chi phí nhân sự cao hơn; hậu quả nghiêm trọng nếu vùng phủ bị đứt                     |
| Mạng lưới tình nguyện viên    | Giảm chi phí trực tiếp, có tính chính danh trong cộng đồng | Khả năng có mặt thất thường, kiệt sức, thiếu giám sát và rủi ro bảo vệ an toàn        |
| Lực lượng lao động có trả phí | Trách nhiệm và thời gian phục vụ rõ hơn                    | Giá cao hơn, khó tuyển người và kinh tế đơn vị yếu ở khu vực thưa dân                 |
| Bảng theo dõi cho gia đình    | Giúp gia đình yên tâm và phối hợp                          | Áp lực từ gia đình, rò rỉ dữ liệu và cảm giác an toàn giả                             |
| Giới hạn địa bàn              | Mật độ phục vụ và giám sát tốt hơn                         | Số người tiếp cận ban đầu thấp hơn, kết quả khó khái quát sang nơi khác               |

## Rủi ro bậc hai khó nhận thấy

- Người thân sống xa có thể dùng dịch vụ mua ngoài để thay thế sự hiện diện và
  trách nhiệm của chính mình.
- Đơn vị cung cấp có thể ưu tiên hộ khỏe hơn, sống gần nhau hơn hoặc khá giả hơn
  để làm đẹp chỉ số.
- Tình nguyện viên có thể âm thầm trở thành một lực lượng chăm sóc lâm sàng
  không được đào tạo và bảo vệ đúng mức.
- Bảng theo dõi có thể khiến một vụ việc chưa giải quyết trông như đã được quản
  lý chỉ vì có người bấm xác nhận tiếp nhận.
- Một thí điểm thành công có thể biến mất khi tài trợ kết thúc, để lại sự lệ
  thuộc nhưng không còn dịch vụ.
- Dữ liệu rủi ro hộ gia đình có thể bị lợi dụng cho gian lận, bóc lột hoặc định
  giá phân biệt.

## Quy tắc quyết định cuối cùng

Chỉ chuyển sang phát triển phần mềm khi một cuộc thẩm định độc lập xác nhận:

1. có thể đo được mẫu số của nhóm mục tiêu
2. sự đồng thuận và quyền tự chủ là có thật
3. mạng lưới hỗ trợ có thể xử lý vụ việc đến khi kết thúc
4. các vụ việc chưa giải quyết vẫn được hiển thị, không bị che khuất
5. kinh tế đơn vị bao gồm đầy đủ chi phí cung cấp dịch vụ con người và giám sát
6. dịch vụ công và cơ sở lâm sàng chấp nhận các trường hợp được chuyển giao
7. dịch vụ vẫn có giá trị ngay cả khi không tuyên bố những lợi ích sức khỏe chưa
   được đo lường
