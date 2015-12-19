## 認証
* https://public-api.wordpress.com/oauth2/authorize?client_id=your_client_id&redirect_uri=your_url&response_type=token へアクセスさせる
  - `your_client_id` - 登録したアプリの Client ID
  - `redirect_uri` - 登録したアプリの Redirect URL
  - `response_type` - **token** でないといけない
* WordPress.com で認証が OK になると、アクセストークンが返ってくる
  - `redirect_url`#access_token=YOUR_API_TOKEN&expires_in=64800&token_type=bearer&site_id=blog_id <- こんなの
