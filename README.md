# Pacman - Reinforcement Learning - Nguyễn Hữu Bằng (18020196)
## Đề bài :  http://ai.berkeley.edu/reinforcement.html

## Điểm autograder
- Question q1: 6/6
- Question q2: 1/1
- Question q3: 5/5
- Question q4: 5/5
- Question q5: 3/3
- Question q6: 1/1
- Question q7: 1/1
- Question q8: 3/3
- Total: 25/25
## Question 1 
- Cài đặt hàm duyệt MDP trong Init: Duyệt các trạng thái tiếp theo:
    + Nếu là trạng thái cuối, trả về số điểm.
    + Nếu không là trạng thái cuối, duyệt các trạng thái tiếp theo, trả về maximun theo transition và decay.
- Cài đặt hàm tính QValue.
- Cài đặt chọn action: Theo policy đạt số điểm cao nhất.
## Question 2:
- Noise = 0 => Bài toán luôn trả về một kết quả với policy dẫn đến việc đi qua cầu (luôn tìm được giải pháp tối ưu)
## Question 3:
- a: Living Reward < 0 nên policy tối ưu luôn ưu tiên việc giảm thời gian tồn tại => Nhanh nhất.
- b: Living Reward = 0 nên agent sẽ chọn đường đi dài hơn.
- c: 0 > Living Reward > 3a nên tỉ lệ mạo hiểm các lựa chọn mới tăng lên.
- d: 0 > Living Reward > 3c nên tỉ lệ mạo hiểm thấp hơn => Chọn ô +10 để tối ưu số điểm.
- e: Living Reward >> Exit Reward nên agent tối đa hóa thời gian tồn tại.
## Question 4:
- Cài đặt để agent học qua việc thử thay vì sử dụng MDP.
- Sử dụng hàm random trong các policy sub-optimal để tăng learning rate.
## Question 5:
- Tương tự Q4, tuy nhiên thay vì random trong các policy sub-optimal thì thi thoảng sẽ chọn random trong toàn bộ policy.
## Question 6:
- Learning rate không tồn tại do iteration quá nhỏ so với success rate.
## Question 7:
- Training với các hàm đã cài đặt trong Q4, Q5.
## Question 8:
- Training với featureVector.
