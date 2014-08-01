PHP TUTORIAL: PAYPAL PAYMENT DATA TRANSFER (PDT)
==========

PayPal Payment Data Transfer(PDT)

使用方法：
1、首先利用如下代码获取Transaction ID

if(isset($_GET['tx']))
{
  $tx = $_GET['tx'];
  // 其他操作
}

2、调用get_payment_data.php中的get_payment_data($tx)函数，如果成功则返回以关联数组组织的交易数据，失败则返回FALSE。

3、更加详细教程请见：
