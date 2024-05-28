## 自用RIME配置 (暂时只放配色)


### 自用配色方案/color_scheme(部分来源于网络)
```yaml
"win11":
  name: Win11
  author: Tom
  text_color: 0x0D0D0D
  back_color: 0xF9F9F9
  border_color: 0xF0F0F0
  shadow_color: 0x304B4B4B #*候选窗投影颜色,默认透明 
  label_color: 0x535353
  hilited_text_color: 0x0D0D0D
  hilited_back_color: 0xF0F0F0
  candidate_text_color: 0x0D0D0D
  comment_text_color: 0x0D0D0D
  hilited_candidate_text_color: 0x0D0D0D
  hilited_comment_text_color: 0x0D0D0D
  hilited_candidate_back_color: 0xF0F0F0
  hilited_label_color: 0x535353
  hilited_mark_color: 0xC06700

"blue_dark":
  author: "木易"
  back_color: 0x36261F
  candidate_text_color: 0xDBDBDB
  comment_text_color: 0xA8A8A8
  hilited_back_color: 0x471885
  hilited_candidate_back_color: 0x63453A
  hilited_candidate_label_color: 0xFFFFFF
  hilited_candidate_text_color: 0xDBDBDB
  hilited_comment_text_color: 0xA8A8A8
  hilited_mark_color: 0xD6D6D6
  hilited_text_color: 0xD6D6D6
  label_color: 0xDBDBDB
  name: "秃秃推荐／蓝黑"
  text_color: 0xD6D6D6

"wechat":
  name: '微信键盘 / WeChat-keyboard' # 配色取自微信键盘
  author: zsakvo
  text_color: 0x424242
  back_color: 0xFFFFFF
  border_color: 0x00FFFFFF
  shadow_color: 0x304B4B4B
  comment_text_color: 0x424242
  label_color: 0x6F6F6F
  # hilited_candidate_back_color: 0x75B100
  hilited_candidate_back_color: 0x74A01C
  hilited_candidate_text_color: 0xFFFFFF
  hilited_comment_text_color: 0xDBDBDB
  hilited_label_color: 0xE5F0D8

"wechat_dark":
  name: '微信键盘 暗色' # 配色取自微信键盘
  author: xuabi
  color_format: "rgba"
  text_color: 0xCCCCCC
  back_color: 0x161B22
  border_color: 0x15151500
  shadow_color: 0x1515154B
  comment_text_color: 0xDBDBDB
  label_color: 0x6F6F6F
  hilited_candidate_back_color: 0x00A86F
  hilited_candidate_text_color: 0xFFFFFF
  hilited_comment_text_color: 0xDBDBDB
  hilited_label_color: 0xE5F0D8

"pornhub":
  name: 'PornHub 配色'
  author: xuabi
  color_format: "rgba"
  text_color: 0xFFFFFF
  back_color: 0x1B1B1B
  border_color: 0x15151500
  shadow_color: 0x1515154B
  comment_text_color: 0xDBDBDB
  label_color: 0xFF9000
  hilited_candidate_back_color: 0xFF9000
  hilited_candidate_text_color: 0x1B1B1B
  hilited_comment_text_color: 0xDBDBDB
  hilited_label_color: 0xFFFFFF

"green":
  name: "浅绿"
  author: xubai 
  back_color: 0xfff4efec
  shadow_color: 0x4B151515 
  border_color: 0x00000000
  hilited_text_color: 0xff483d37
  hilited_label_color: 0xff6a564c
  hilited_candidate_text_color: 0xff483d37
  hilited_comment_text_color: 0xff483d37
  hilited_candidate_back_color: 0xffbbbc8f
  label_color: 0xff6a564c
  candidate_text_color: 0xff483d37
  comment_text_color: 0xff483d37
```
### 配色预览
![配色预览](/assets/color_schema.png "配色预览")

### 样式/style
```yaml
style:
  label_format: "%s"
  inline_preedit: true
  font_point: 16
  label_font_point: 12
  horizontal: true
  layout:
    max_height: 0
    max_width: 1200
    min_width: 10
    margin_x: 10
    margin_y: 8
    spacing: 16
    candidate_spacing: 24
    hilite_spacing: 6
    hilite_padding: 3
    hilite_padding_x: 5
    corner_radius: 8
    round_corner: 8
    shadow_radius: 4
```

### 使用方式
小狼毫(Weasel): 在用户文件夹/weasel.custom.yaml中添加以下内容(若已有内容，自行修改):
```yaml
patch:
  style/horizontal: false # true为横排，false为竖排
  style/color_scheme: wechat  # 配色名称
  style:
    # 填入上方style内容
    
  preset_color_schemes:
    # 填入上方配色内容
    "win11":
      ....
    "blue_dark":
      .... 
```
