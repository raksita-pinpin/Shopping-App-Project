# cs211-641-project

## รายชื่อสมาชิก
* (6310450701) (ศุภกิจ สุขสมศรี) (raysupakit138)
  * ออกแบบและทำหน้า gui ใน sceneBuilder ทั้งหมด และช่วยทำโค้ดในโปรแกรมเชื่อมหน้าแต่ละหน้า
  * เพิ่มรหัสผ่าน admin และ เขียน models User , UserList , UserFileDataSource และ เขียนไฟล์ userAccount.csv
  * เพิ่มเวลาในการล็อกอินของ user (lastLoginTime) และแก้บัคหน้า register ในบางส่วน รวมถึงการ Login
  * เพิ่มหน้าข้อมูลผู้ใช้งานระบบและเพิ่มฟังก์ชันการอัพโหลดรูปในตอนที่สมัครใช้งานและเพิ่มเป็น default picture กรณีไม่อัพโหลดรูป
  * สร้างไฟล์ .jar เพื่อใช้ในการรันโปรแกรม
* (6310450581) (นิธิโชติ ขาวผ่อง) (pee0071)
  * ช่วยออกแบบหน้า GUI และใส่รูปภาพ และ เขียนโค้ดปุ่ม Back Next และ Confirm ให้ครบทุกหน้า
  * เพิ่มการตั้งค่าสินค้า shopSetting ในส่วนของController/Models/Service เเละเขียนไฟล์ shopSetting.csv
  * เพิ่มการลงสินค้า sellHere ในส่วนของController/Models/Service เเละเขียนไฟล์ sellHeres.csv
  * เมื่อสมัครขายสินค้าเเอคเค้านั้นจะกลายเป็นผู้ขายทันที
  * เพิ่มหน้าที่สามารถดูได้ว่าสินค้าของร้านเหลือเท่าไหร่เเล้วละถ้าของใกล้หมดจะมีไอคอนเเจ้งเตือน
* (6310450654) (รักษิตา รัตนาลังการ) (raksita-pinpin)
  * ร่างแผนผัง Project และช่วยคิดรูปแบบ GUI และ เขียนโค้ดปุ่ม Back Next และ Confirm ให้ครบทุกหน้า
  * เพิ่มหน้าร้าน MarketPlaceController เพื่อให้ผู้คนสามารถมาซื้อสินค้าได้ เเละสามารถดูได้ว่าคนไหนบ้างที่ซื้อของจากร้านค้า shopHistory เเละเขียนไฟล์ shopHistory.csv
  * เพิ่มช่องที่สามารถเลือกได้ว่าอยากหาสินค้าราคามากไปน้อย น้อยไปมากเเละสามารถดูวันที่สินค้าเก่าใหม่ได้ SorceByPriceAsc.java,SorceByPriceDesc.java และออกแบบใน FXML
  * เมื่อกดซื้อสินค้าจะมีหน้าอีกหน้าเเสดงผลออกมาเพื่อยืนยันว่าจะซื้อสินค้า paymentPopupController
  * เมื่อซื้อสินค้าเเล้วสามารถไปดูสินค้าที่ซื้อไว้ได้ OrderStatusController

## วิธีการติดตั้งหรือรันโปรแกรม
เมื่อ clone โปรแกรมลงมาแล้ว ในโฟลเดอร์ gradedog จะมีไฟล์ Ku-mall.jar เพื่อใช้เปิดโปรแกรม
หากรันไม่ได้ให้เปิดโปรแกรม command prompt ละ cd เข้าหาโฟลเดอร์ที่เก็บไฟล์ jar และ ใช้คำสั่ง java -jar Ku-mall.jar

## การวางโครงสร้างไฟล์
* (project-641-gradedog)
  * (data_csv)
    * sellHeres.csv(เก็บข้อมูลสินค้าที่ลงขายทั้งหมด)
    * shopHistory.csv(เก็บข้อมูลประวัติการซื้อของทั้งหมด)
    * shops.csv(เก็บข้อมูลของผู้ใช้ระบบทั้งหมด)
    * shopSetting.csv(เก็บข้อมูลการตั้งค่าจำนวนสินค้าเเละเเสดงสัญลักษณ์เเจ้งเตือนว่าของกำลังจะหมด)
    * userAccount.csv(เก็บข้อมูล)
  * (Controller)
    * AdminInformationController
    * ItemCardController
    * ItemsBoxShopController
    * LoginAdminController
    * LoginController
    * LoginUserController
    * MarketPlaceController
    * OrderStatusBoxController
    * OrderStatusController
    * PaymentPopupController
    * Primary Controller
    * RegisterController
    * SecondaryController
    * SelectedItemController
    * SellHereController
    * ShopDetailController
    * ShopItemsController
    * ShoppingOrSoldController
    * ShopSettingController
    * UserBoxController
    * UserInformationController
  * (Interfaces)
    * ItemCardListener
  * (models)
    * Item
    * ItemList
    * Shop
    * ShopDetailList
    * ShopHistory
    * ShopHistoryList
    * ShopSetting
    * ShopSettingList
    * User
    * UserList
  * (Service)
    * CreateDateTime
    * DataSource
    * ImageUploadService
    * ItemFileData Source
    * ItemRepository
    * ItemsBoxShopService
    * LoginAdminService
    * LoginUserService
    * MarketPlaceService
    * OrderStatusService
    * PaymentPopupService
    * SelectedItemService
    * SellHereService
    * ShopDetailFileDataSource
    * ShopDetailService
    * ShopHistoryFileDataSource
    * ShopHistoryRepository
    * ShopItemsService
    * ShoppingSoldService
    * ShopRepository
    * ShopSettingFileDataSource
    * ShopSettingRepository
    * ShopSettingService
    * SortByDateDesc
    * SortByPriceAsc
    * SortByPriceDesc
    * UserFileDataSource
    * UserInformationService
    * UserRepository
    * UserSession
  * image
    * icons(เก็บรูปในส่วนของภาพสัญลักษณ์ขนาดเล็ก)
    * Items(เก็บรูปในส่วนของรูปสินค้าทั้งหมดของเเอพลิเคชั่น)
    * users(เก็บรูปในส่วนของผู้ใช้งานระบบ)
      * image ในส่วนต่างๆ
  * KU-mall (executable file ของเเอพลิเคชั่น)

## ตัวอย่างข้อมูลผู้ใช้ระบบ
* (admin) username : testadmin password : 1234
* (admin) username : adminray password : 12345
* (admin) username : adminpin password : 12345
* (admin) username : adminp password : 12345
* (seller) username : Supakit password : 12345
* (seller) username : Nitichot password : 1234
* (seller) username : Raksita password : 12345
* (buyer) username : testuser password : 12345
* (buyer) username : testuser2 password : 12345
* (buyer) username : testuser3 password :1234


## สรุปสิ่งที่พัฒนาแต่ละครั้งที่นำเสนอความก้าวหน้าของระบบ
* ครั้งที่ 1 (11/08/64)
  * (ออกแบบและทำหน้าโปรแกรมใน scene builder และ fxml) (ศุภกิจ สุขสมศรี)
  * (ออกแบบและทำหน้าโปรแกรมใน scene builder และ fxml) (นิธิโชติ ขาวผ่อง)
  * (ออกแบบและทำหน้าโปรแกรมใน scene builder และ fxml) (รักษิตา รัตนาลังการ)
* ครั้งที่ 2 (11/09/64)
  * (เพิ่มรหัสผ่าน admin และ เขียน models User , UserList , UserFileDataSource และ เขียนไฟล์ userAccount.csv) (ศุภกิจ สุขสมศรี)
  * (เขียน models Shop , ShopList , ShopDetailList , ShopDetailFileSource และ เขียนไฟล์ shops.csv) (นิธิโชติ ขาวผ่อง)
  * (เขียน models SellHere , SellHereList , SellHereFileDataSource และเขียนไฟล์ sellHeres.csv) (รักษิตา รัตนาลังการ)
* ครั้งที่ 3 (28/09/64)
  * ( Controller)
    - AdminInformationController ,LoginAdminController ,LoginController ,LoginUserController ,RegisterController ,UserInformationController)
  * ( Services)
    - CreateDadeTime ,UserSession
    - Add fxml และระบบ userService ต่างๆ (ศุภกิจ สุขสมศรี)
  * ( Controller)
    - ItemsBoxShopController ,SellHereController ,ShopDetailController ,ShopItemsController ,ShopSettingController
  * ( Models)
    - Item ,ItemList ,ShopDetailList ,ShopSetting ,ShopSettingList
  * ( Service)
    - ItemFileDataSource ,ShopSettingFileDataSource
    - Add fxml ส่วนต่างๆ (นิธิโชติ ขาวผ่อง)
  * ( Controller)
    - ConfirmOrderController ,ItemCardController ,MarketPlaceController ,OrderStatusController ,OutOfStockController ,ProductDetailController
      ,SelectedItemController ,ShoppingController
  * ( Models)
    - Shop ,ShopDetailList
  * ( Service)
    - ShopDetailFileDataSource
    - Add fxml ต่างๆ (รักษิตา รัตนาลังการ)
* ครั้งที่ 4 (21/10/64)
  *(controller)
  -LoginAdminController ,LoginController
  -LoginUserController ,UserBoxController
  -RegisterController
  *(models)
  -User ,UserList
  *(services)
  -ImageUploadService ,CreateDateTime ,DataSource
  -LoginAdminService ,LoginUserService ,SortByDateDesc
  -UserFileDataSource ,UserInformationService
  -UserRepository ,UserSession
  *Update fxml
  *css (ตกแต่งหน้าGUI)  (ศุภกิจ สุขสมศรี)
  
  *(controller)
  -ItemsBoxShopController ,ShopDetailController
  -ShopItemsController ,ShoppingOrSoldController ,ShopSettingController
  *(models)
  -Shop
  *(services)
  -ImageUploadService ,ItemFileDataSource ,ItemRepository
  -ItemsBoxShopService ,SellHereService ,ShopDetailService
  -ShopHistoryFileDataSource ,ShopHistoryRepository ,ShopItemsService
  -ShoppingOrSoldService ,ShopRepository ,ShopSettingFileDataSource
  -ShopSettingRepository ,ShopSettingService
  *(Update fxml)
  *css (ตกแต่งหน้าGUI)  (นิธิโชติ ขาวผ่อง)

  *(controller)
  -ItemCardController ,MarketPlaceController ,OrderStatusBoxController
  -OrderStatusController ,OutOfStockController ,PaymentPopupController
  -ProductDetailController ,SelectedItemController ,ShopSettingController
  *(models)
  -ShopHistory ,ShopHistoryList
  *(services)
  -MarketPlaceService ,OrderStatusService
  -PaymentPopupService ,SelectedItemService-ShopSettingFileDataSource
  -ShopSettingRepository ,ShopSettingService
  -SortByPriceAsc ,SortByPriceDesc
  *(Update fxml)
  *css (ตกแต่งหน้าGUI)  (รักษิตา รัตนาลังการ)
  # Shopping-App-Project
