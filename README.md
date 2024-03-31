<div align="center">

<h1>BOS Bootcamp</h1>
<strong>Học cách phát triển giao diện người dùng với Blockchain Operating System</strong>
<p align="center">
    <br />
    <a href="https://www.openedu101.com/">
        <img src=".github/images/takethiscourse.png" width="200" h alt=""/></a>
    <br />
</p>
Chào mừng bạn đến với repository của khoá học BOS Bootcamp. <br/> Khoá học này được phát triển bởi <a href="https://www.openedu101.com/">OpenEdu101</a> và được tài trợ bởi <a href="https://near.org/">Near Foundation</a>. <br> Trình bày, cập nhật nội dung bởi
<a href="https://www.youtube.com/channel/UC0QESw8LTPb841qcABmOsvA">terrancrypt</a>.
</div>

<br/>

Chào mừng bạn đến với Series BOS Bootcamp! Trong khoá học này, chúng ta sẽ khám phá BOS Component, một khái niệm của NEAR Blockchain, và tìm hiểu cách nó đóng góp cho sự phát triển của Web3. 

- [Tài nguyên](#tài-nguyên)
- [Yêu cầu](#yêu-cầu)
- [Section 1: Xây dựng BOS Component đầu tiên](#section-1-xây-dựng-bos-component-đầu-tiên)
  - [BOS Component là gì?](#bos-component-là-gì)
  - [Tại sao nên sử dụng BOS Component?](#tại-sao-nên-sử-dụng-bos-component)
  - [BOS Component nằm ở đâu trong một hệ thống blockchain?](#bos-component-nằm-ở-đâu-trong-một-hệ-thống-blockchain)
  - [Xây dựng BOS Component đầu tiên](#xây-dựng-bos-component-đầu-tiên)
  - [Kết luận và hướng dẫn tiếp theo](#kết-luận-và-hướng-dẫn-tiếp-theo)
- [Section 2: Tương tác với smart contract](#section-2-tương-tác-với-smart-contract)
  - [Cách tương tác với NEAR blockchain](#cách-tương-tác-với-near-blockchain)
  - [Cách tương tác với EVM blockchain](#cách-tương-tác-với-evm-blockchain)
- [Section 3: Design Component](#section-3-design-component)

# Tài nguyên

- **Wallet**
  - [Meteor Wallet](https://meteorwallet.app/)
  - [My Near Wallet](https://www.mynearwallet.com/)

- **Faucet**
  - [Near Faucet](https://near-faucet.io/)

- **Documentation**
  - [NEAR Component Documentation](https://docs.near.org/bos/tutorial/quickstart)

# Yêu cầu

- **HTML, CSS, JavaScript**
  - [Frontend Web Development Bootcamp Course (JavaScript, HTML, CSS)](https://www.youtube.com/watch?v=zJSY8tbf_ys)
  - [HTML, CSS từ Zero Tới Hero - F8](https://www.youtube.com/watch?v=R6plN3FvzFY&list=PL_-VfJajZj0U9nEXa4qyfB4U5ZIYCMPlz)
- **React**
  - [Front End Development Libraries - Freecodecamp](https://www.freecodecamp.org/learn/front-end-development-libraries/)
  - [Meta Front-End Developer Professional Certificate](https://www.coursera.org/professional-certificates/meta-front-end-developer)



# Section 1: Xây dựng BOS Component đầu tiên
_[⭐️ Video #1: Xây dựng BOS Component đầu tiên](https://youtu.be/VU-E30-urYI)_

Video giới thiệu về ý nghĩa của BOS, cách nó hoạt động trong hệ thống Web3, và tại sao nó quan trọng trong việc giải quyết những thách thức của Web2. Hướng dẫn chi tiết cách xây dựng BOS Component, với yêu cầu kiến thức cơ bản về HTML, CSS, JavaScript và React. 

Video chia thành các phần WHY, WHAT, WHERE, và HOW để giải thích mục đích, khái niệm, vị trí, và cách xây dựng BOS Component.

Cuối cùng, mình khuyến khích bạn tự nghiên cứu các ngôn ngữ và công cụ liên quan để tham gia vào việc xây dựng một hệ sinh thái front-end phi tập trung kết nối với nhiều blockchain khác nhau. Khám phá những cơ hội mới trong thế giới phức tạp của blockchain và Web3!

## BOS Component là gì?
[NEAR Component Documentation](https://docs.near.org/bos/tutorial/quickstart)

- **BOS (Blockchain Operating System)**: Một khái niệm của NEAR Blockchain, còn được gọi là NEAR Components.

- **Component**: Là một thành phần trong lập trình front-end, trong trường hợp này, được xây dựng để tương tác với nhiều blockchain khác nhau.

## Tại sao nên sử dụng BOS Component?
- **Lịch sử Phát triển Web**: So sánh giữa Web1, Web2, và Web3.
- **Web3**: Tập trung vào sự phi tập trung, ẩn danh và sự tương tác trực tiếp với blockchain.
- **Yếu tố của BOS Component**:
  - **Tổng hợp**: Có thể truy cập tất cả các component thông qua gateway.
  - **Tái sử dụng**: Có thể sử dụng lại các component đã xây dựng.
  - **Phi tập trung**: Mã nguồn của component được lưu trữ trên blockchain.
- **Web3 và vấn đề của Web2**:
  - Web2 tập trung dữ liệu và có thể gây mất an toàn thông tin cá nhân.
  - Web3 giải quyết vấn đề này thông qua ẩn danh và phi tập trung.
- **Mô hình hoạt động của dApps trong Web3**:
  - Sử dụng smart contract và blockchain để xử lý logic.
  - Sử dụng mạng lưới lưu trữ phi tập trung như IPFS để lưu trữ dữ liệu lớn.
  - Sử dụng server tập trung lưu trữ code front-end.
- **Vai trò của BOS trong hệ thống**:
  - Smart contract xử lý logic + code front-end.
  - IPFS lưu trữ dữ liệu lớn.

## BOS Component nằm ở đâu trong một hệ thống blockchain?

- **Gateway và Modules**:
  - Mô tả cách gateway tổng hợp các module và thư viện hỗ trợ các component.
  - Mô tả module Wallet Library và thư viện hỗ trợ kết nối với blockchain.
- **BOS Application**:
  - BOS Application là tập hợp của tất cả các component, được bao bọc bởi môi trường BOS.
  - Mỗi component được xem như một widget.

[Potlock](https://near.org/potlock.near/widget/Index) | [Potlock Github Repository](https://github.com/PotLock/bos-app)

## Xây dựng BOS Component đầu tiên
- [Meteor Wallet](https://meteorwallet.app/)
- [My Near Wallet](https://www.mynearwallet.com/)
- [Near Faucet](https://near-faucet.io/)
- [Near Social](https://near.social/)

## Kết luận và hướng dẫn tiếp theo
- Mục tiêu của BOS là tạo ra một hệ sinh thái front-end có thể tương tác với nhiều blockchain và được xây dựng với tính phi tập trung.
- Video chỉ là bắt đầu, sẽ có nhiều phần khác với nhiều yếu tố và công cụ khác nhau.
- Tự tìm hiểu HTML, CSS, JavaScript và React là quan trọng trước khi bắt đầu.

# Section 2: Tương tác với smart contract
_[⭐️ Video #2: Tương tác với Smart Contracts](https://youtu.be/UpKSOrYPo7M)_


Phần này tập trung vào việc tạo các BOS component để giao tiếp với các blockchain khác nhau. Sử dụng `near-api-js` để tương tác với NEAR blockchain và `ethers.js` để tương tác với các blockchain tương thích với EVM.

## Cách tương tác với NEAR blockchain

Contract dùng để tương tác: [guest-book.terrancrypt.testnet](https://testnet.nearblocks.io/address/guest-book.terrancrypt.testnet)

- [Nearblocks](https://testnet.nearblocks.io/)
- [Interacting with NEAR documennt](https://docs.near.org/bos/api/near)
- [Jutsu AI](https://jutsu.ai/)

Component hoàn thiện trong phần này: [GuestBook](https://test.near.org/terrancrypt.testnet/widget/BOSBootcamp-GuestBook)

## Cách tương tác với EVM blockchain

Contract dùng để tương tác: [0xc5b16a21c3ceca9a43898886d4d075612c6c917d](https://mumbai.polygonscan.com/address/0xc5b16a21c3ceca9a43898886d4d075612c6c917d)

- [Metamask](https://docs.metamask.io/)
- [Mumbai Faucet](https://www.alchemy.com/faucets/polygon-mumbai)
- [Mumbai Network](https://chainlist.org/?search=mumbai&testnets=true)
- [Mumbai Explorer](https://mumbai.polygonscan.com/) 
- [NEAR for Ethereum developers documennt](https://docs.near.org/bos/tutorial/ethers-js)

Component hoàn thiện trong phần này: [EVM Factory](https://test.near.org/terrancrypt.testnet/widget/BOSBootcamp-EVMFactory)

# Section 3: Design Component

_[⭐️ Video #3: Design Component](https://youtu.be/SnxH1_J_tGA)_'

Component hoàn thiện trong phần này: [StyledEVMFactory](https://test.near.social/terrancrypt.testnet/widget/BOSBootcamp-StyledEVMFactory)

(Updating...)
 