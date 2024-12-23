<template>
    <div class="footer">   
        <div class="footer-left">
            <div class="footer__content logo">
            <img src="../../assets/image/logo.png" width="250" height="60" alt="">
        </div>
        <div class="footer__content">
            <div class="icon-boder"><i class="fas fa-phone-alt"></i></div>
            <span>0983 784 509</span>
        </div>
        <div class="footer__content">
            <div class="icon-boder"><i class="fas fa-map-marker-alt"></i></div>
            <span>Số 62, đường Xuân Đỉnh, Phường Xuân Tảo, Quận Bắc Từ Liêm, Tp. Hà Nội</span>
        </div>
        <div class="footer__content">
            <div class="icon-boder"><i class="fas fa-envelope"></i></div>
            <span>MyPenguOffice@gmail.com</span>
        </div>
        </div>
        <div class="footer-right">
            <div class="text-group">
                <h2>Dịch vụ</h2>
                <p>Điều khoản sử dụng</p>
                <p>Chính sách bảo mật</p>
                <p>Chính sách thanh toán</p>
                <p>Giới thiệu</p>
                <p>Hệ thống cửa hàng</p>
            </div>
            <div class="text-group">
                <h2>Hỗ trợ</h2>
                <p>Chính sách đổi trả</p>
                <p>Chính sách bảo hành</p>
                <p>Chính sách vận chuyển</p>
            </div>
            <div class="text-group">
                <h2>Tài khoản</h2>
                <p>Tài khoản của tôi</p>
                <p>Thay đổi thông tin</p>
                <p>Lịch sử mua hàng</p>
            </div>
        </div>
    </div>
</template>
<style scoped>
.footer{
    display: flex;
    padding: 60px 0;
    background: #fff;
    margin: 0 15%;
    border-radius: 10px;
}
.footer-left{
    padding: 0 30px;
    width: 35%;
    display: flex;
    flex-direction: column;
    border-right: 1px solid #ccc;
}
.footer-right{
    padding: 0 30px;
    width: 65%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
.footer-right h2, p {
    padding: 10px 0;
}
.footer__content{
    display: flex;
    gap: 7px;
    align-items: center;
    padding: 10px 0;
}
.icon-boder{
    width: 25px;
    height: 25px;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid #000;
    border-radius: 4px;
}
</style>