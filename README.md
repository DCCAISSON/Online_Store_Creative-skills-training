# GitHub Pages 网站使用说明

这是一个用于展示真实“创意设计职业技能培训”课程的静态单页网站。它适合在 PayPal 店铺链接一栏填写为公开可访问的独立网站，但页面内容必须与实际提供的培训一致。

## 上传前必须修改

打开 `index.html`，搜索并替换以下内容：

1. 页面标题和页脚
   - 如果你使用个人名义提供培训，请改成你的真实姓名或真实使用的个人品牌。
   - 如果没有注册公司，不要使用容易让人误认为已注册公司的表述。

2. 联系邮箱
   - 将“请填入真实联系邮箱”改成与 PayPal 账户一致、可以正常收信的邮箱，并设置对应的 `mailto:` 链接。

3. Course tuition
   - USD 80 / USD 150 是当前页面沿用的起价示例，发布前必须改成真实课程学费。

4. Courses
   - 只保留你实际提供的课程、课时、练习项目和反馈方式。
   - 不要声称提供学历、职业资格或官方认证，除非你确实拥有相应资质。

## 发布到 GitHub Pages

最简单方式：

1. 登录 GitHub。
2. 新建仓库，仓库名填写：
   `你的GitHub用户名.github.io`
3. 将 `index.html` 和 `styles.css` 上传到仓库根目录。
4. 打开仓库 `Settings` → `Pages`。
5. 在 Build and deployment 中选择 `Deploy from a branch`。
6. Branch 选择 `main`，目录选择 `/ (root)`。
7. 保存后，你的网站地址通常是：
   `https://你的GitHub用户名.github.io/`

## 自定义域名（可选）

如果你已经购买自己的域名，例如 `yourname.com`：

1. GitHub 仓库 Settings → Pages → Custom domain。
2. 填写你的域名。
3. 按 GitHub 给出的 DNS 指引，在域名服务商处配置 DNS。
4. DNS 生效后开启 HTTPS。

建议先把 GitHub Pages 原始地址跑通，再绑定自定义域名。

## PayPal 填写建议

如果实际业务是创意设计技能培训，商户行业分类应选择与职业技能培训相符的分类；“店铺链接”填写公开可访问的主页 URL，例如 `https://你的用户名.github.io/仓库名/`。

网页内容应与实际收付款业务一致。不要虚构公司、学员、资质、课程、交易记录或不存在的商品。
