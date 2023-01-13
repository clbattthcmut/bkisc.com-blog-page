# BKISC Blog-News-Event Page
## Netlify
Đang deploy ở https://eclectic-belekoy-9c31db.netlify.app

## Requirement
- Cần tải golang về máy tại [đây](https://go.dev/dl/)
- Cần tải hugo extended bằng bản binary tại [đây](https://github.com/gohugoio/hugo/releases/tag/v0.109.0)

**Note**: nếu như sử dụng Unix based, có thể cài đặt thông qua các package manager như **apt** hoặc **brew** và có thể cài đặt trên [**docker**](https://gohugo.io/installation/linux/#docker) (không official)

## Installation

Clone repo về máy -> Vào thư mục git -> Chạy lệnh hugo

```bash
git clone --recurse-submodules -j8 https://github.com/clbattthcmut/bkisc.com-blog-page.git
cd bkisc.com-blog-page

# Hiện content nháp (trên front matter có draft: true)
hugo server -D -w

# Không hiện content nháp
hugo server -w
```

## Hướng dẫn đóng góp nội dung cho trang Blog
### Format file
Thành viên câu lạc bộ cần thêm tên mình vào danh sách member trước khi contribute blog
- Hướng dẫn add tên mình vào danh sách member tại [đây](./content/authors/README.md)
- Hướng dẫn đóng góp blog tại [đây](./content/blog/README.md)

Ngoài ra trang web có hai mục /news và /events để đăng tin tức hoặc thông báo sự kiện sắp diễn ra, các bài đăng trong mục này sẽ để dưới tên là admin BKISC và do bạn Chủ Tịch CLB viết.
- Hướng dẫn đăng tin tức tại [đây](./content/post/README.md)
- Hướng dẫn đăng thông báo sự kiện tại [đây](./content/event/README.md)

### Về commit message
**Note**: mong mọi người commit 1 lần sau mỗi hoạt động trên với message phản ánh commit đó (cái này chỉ là gợi ý thôi, mọi người cứ commit message thoải mái nha, cái nào hài hài xíu)
```
[<Add, Delete, Modify>] [<Blog, News, Events, Member>] [<Tên file/thư mục liên quan>]
```
Ví dụ: 
```
[Add] [Member] [hdthinh1012]
[Modify] [Blog] [duti/sekai-ctf-2022-bottle-poem]
[Add] [Events] [2022-09-05-thaidn-talk]
```