Customer(MaKH, HoTen, Email, Sdt, DiaChi)
Product(MaSP, TenSP, Gia, MoTa, LoaiHang)
Staff(MaNV, HoTen, ViTri, NgayVaoLam)
Order(MaDon, NgayDatHang, TongTien, TrangThai, MaKH FK->Customer, MaNV FK->Staff)
OrderDetail(SoLuong, DonGia, MaDon FK->Order, MaSP FK->Product, --PK(MaDon, MaSP))

* DonGia(OrderDetail) là giá tại thời điểm KH mua sp. Còn Gia(Product) là giá có thể thay đổi được
