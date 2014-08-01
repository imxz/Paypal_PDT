###PHP TUTORIAL: PAYPAL PAYMENT DATA TRANSFER (PDT)

####描述
Payment Data Transfer (PDT) is a secure method to retrieve the details about a PayPal transaction so that you can display them to your customer. It is used in combination with PayPal Payments Standard, so that after a customer returns to your website after paying on the PayPal site, they can instantly view a confirmation message with the details of the transaction.


简单来说，就是在PayPal支付完成后获取交易信息。


####使用方法：
1、首先利用如下代码获取Transaction ID


    if(isset($_GET['tx']))
    {
      $tx = $_GET['tx'];
      // 其他操作
    }


2、调用get_payment_data.php中的get_payment_data($tx)函数，如果成功则返回以关联数组组织的交易数据，失败则返回FALSE。


3、更加详细教程请见：http://ethanblog.com/tech/webdev/php-for-paypal-payment-data-transfer.html
