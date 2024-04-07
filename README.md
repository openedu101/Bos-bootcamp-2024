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

Chào mừng bạn đến với BOS Bootcamp, nơi bạn sẽ khám phá cách phát triển giao diện người dùng (GUI) thông qua Blockchain Operating System (BOS). 

Trong khoá học, bạn sẽ học về ý nghĩa của BOS và cách nó hoạt động trong hệ thống Web3. Bạn sẽ tìm hiểu về BOS Component - một khái niệm quan trọng của NEAR Blockchain - và cách nó đóng góp vào sự phát triển của Web3.

Ngoài ra, bạn sẽ được hướng dẫn cách xây dựng BOS Component đầu tiên, tương tác với smart contract trên NEAR Blockchain và các blockchain tương thích với EVM. Khoá học cũng tập trung vào thiết kế component đẹp mắt và chức năng thông qua CSS, cùng với việc áp dụng mẫu thiết kế component đa blockchain.

Đối tượng của khoá học này là những ai quan tâm đến phát triển giao diện người dùng và blockchain, cũng như muốn hiểu sâu hơn về cách BOS có thể thay đổi cách chúng ta tương tác trực tiếp với công nghệ.

Nếu bạn muốn khám phá cơ hội mới trong thế giới phức tạp của blockchain và Web3, hãy tham gia ngay vào BOS Bootcamp!

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
- [Section 4: Chain-Agnostic Component Design Pattern](#section-4-chain-agnostic-component-design-pattern)
  - [Tại sao blockchain agnostic lại quan trọng?](#tại-sao-blockchain-agnostic-lại-quan-trọng)
  - [Tại sao có một tư duy về component design pattern lại quan trọng?](#tại-sao-có-một-tư-duy-về-component-design-pattern-lại-quan-trọng)

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

_[⭐️ Video #3: Design Component](https://youtu.be/SnxH1_J_tGA)_

Trong phần trước, chúng ta đã tìm hiểu về cách các component tương tác với các smart contract như thế nào. Trong phần này, chúng ta sẽ tìm hiểu làm sao để design các component đó, hay là css trong các BOS component.

Nếu như HTML là một bộ khung xương, phần logic chúng ta viết bằng Javascript là một bộ não, thì bây giờ chúng ta còn thiếu phần làm đẹp cho một component.

Cần component đẹp hơn thì chúng ta cần phải css cho nó, NEAR cung cấp cho cho chúng ta các cách để chúng ta có thể thiết kế được component của chúng ta. 

Component hoàn thiện trong phần này: [StyledEVMFactory](https://test.near.social/terrancrypt.testnet/widget/BOSBootcamp-StyledEVMFactory)

# Section 4: Chain-Agnostic Component Design Pattern

Contract address để sử dụng trong phần này:
- Polygon Mumbai: [0xc5b16a21c3ceca9a43898886d4d075612c6c917d](https://mumbai.polygonscan.com/address/0xc5b16a21c3ceca9a43898886d4d075612c6c917d)
- Arbitrum Sepolia: [0x7DFdCaE1e6a90be0b3CD10e949cE30b137Da58f4](https://sepolia.arbiscan.io/address/0x7DFdCaE1e6a90be0b3CD10e949cE30b137Da58f4)
- Base Sepolia: [0xF4F18A60Af4E5fe47c193CF9603bF82544C0B617](https://sepolia.basescan.org/address/0xf4f18a60af4e5fe47c193cf9603bf82544c0b617)

Phần này chúng ta sẽ nói về Chain-Agnostic Component Design Patterns, hay là mẫu thiết kế component theo kiểu blockchain bất khả tri. 

Mẫu thiết kế (Design pattern) là một kỹ thuật lập trình được sử dụng để giải quyết các vấn đề phổ biến trong thiết kế phần mềm. Chúng cung cấp một cách tiếp cận cấu trúc hợp lý và linh hoạt để xây dựng các hệ thống phức tạp. Mỗi mẫu thiết kế đều mô tả một vấn đề cụ thể cùng với cách giải quyết cho vấn đề đó.

Chain Agnostic hay Blockchain Agnostic là một khái niệm còn khá mới. Khái niệm này nói về việc xây dựng hạ tầng cho một blockchain, ở đây chúng ta có thể gọi là các giải pháp về Blockchain-Agnostic hoặc cách để xây dựng một cơ sở hạ tầng Blockchain-Agnostic. Điều này đơn giản là đề cập đến một cách xây dựng cơ sợ hạ tầng không phụ thuộc vào một blockchain duy nhất mà có thể hoạt động và hỗ trợ nhiều blockchain khác nhau. Bạn có thể thấy những ứng dụng Web3 như Aave hay Metamask có thể hoạt động trên nhiều blockchain khác nhau tương thích với EVM. 

## Tại sao blockchain agnostic lại quan trọng?
- Đầu tiên là giúp các dự án có thể truy cập được thị trường cryptocurrency trên toàn bộ hệ sinh thái web3.
- Thứ hai là giúp bảo vệ dự án trong tương lai.
- Cuối cùng là để chúng ta có thể tận dụng được những ưu điểm của các blockchain khác nhau.

## Tại sao có một tư duy về component design pattern lại quan trọng?
- **Modularity & Reusauble - Tính Mô-đun và Tái Sử Dụng:** Các component được thiết kế để độc lập và có thể sử dụng lại. Thay vì phải xây dựng lại từ đầu, các component có thể được sử dụng lại trong nhiều phần của ứng dụng hoặc thậm chí trong các dự án khác. Điều này giúp giảm thiểu thời gian và công sức cần thiết cho việc phát triển và bảo trì các dự án BOS.
- **Maintainability and Readability, Dễ Bảo Trì và Dễ Đọc:** Mỗi component tập trung vào một chức năng cụ thể của application, làm cho quá trình bảo trì trở nên dễ dàng hơn. Khi cần thay đổi hoặc cập nhật một tính năng cụ thể, chỉ cần tập trung vào component đó mà không ảnh hưởng đến các phần khác của hệ thống. Điều này giảm thiểu nguy cơ gây ra lỗi hoặc tác động không mong muốn lên toàn bộ ứng dụng.
- **Collaboration - Sự Hợp Tác:** Tư duy về component design pattern cho phép các nhóm phát triển làm việc độc lập trên các component khác nhau của ứng dụng. Các nhóm có thể phát triển và kiểm tra các thành phần một cách độc lập trước khi tích hợp chúng lại với nhau. Điều này tạo điều kiện cho sự linh hoạt và hiệu suất trong quá trình phát triển.
- **Disverabitily -  Khả Năng Khám Phá:** Các component sẽ được tổ chức một cách logic và có tài liệu rõ ràng, giúp cho việc tìm kiếm và hiểu được chúng trở nên dễ dàng hơn. Khi cần thiết, các nhà phát triển có thể dễ dàng tìm kiếm và tái sử dụng các thành phần đã được phát triển trước đó thay vì phải xây dựng lại từ đầu.

Component hoàn thiện trong phần này: [StorageFactoryMultiEVM](https://test.near.social/terrancrypt.testnet/widget/StorageFactoryMultiEVM)

(Updating...)
 