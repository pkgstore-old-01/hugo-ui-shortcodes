# Information

Base shortcodes for Hugo.

## Install

```
git submodule add https://github.com/marketplace-hugo/hugo-ui-shortcodes.git themes/ui-shortcodes
```

## Update

```
git submodule update --remote
```

## Uninstall

```
git submodule deinit -f themes/ui-shortcodes && git rm -r --cached themes/ui-shortcodes && rm -rf .git/modules/themes/ui-shortcodes
```

## Codes

### Abbr

```
{{< abbr "[ATTR]" "[ATTRIBUTE]" >}}
```

### Alert

```
{{< alert >}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis id neque a dolor ornare porttitor. Maecenas id est magna. Vivamus ut urna orci. Suspendisse quam lacus, volutpat vitae lectus quis, malesuada tempus magna. Ut cursus vel quam sit amet condimentum. Nam at dignissim dolor. Cras egestas lectus in odio auctor.
{{< /alert >}}
```

```
{{< alert "[TYPE]" >}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis id neque a dolor ornare porttitor. Maecenas id est magna. Vivamus ut urna orci. Suspendisse quam lacus, volutpat vitae lectus quis, malesuada tempus magna. Ut cursus vel quam sit amet condimentum. Nam at dignissim dolor. Cras egestas lectus in odio auctor.
{{< /alert >}}
```

#### TYPE

- `primary`
- `secondary`
- `success`
- `danger`
- `warning`
- `info`
- `light`
- `dark`

### Categories

```
{{< categories >}}
```

### Contact Form

Форма для отправки сообщений по электронной почте автору сайта.

## Syntax

```
{{< form-contact subject="" token="" >}}
```

## ru.toml

```toml
[form.contact.name]
other = "Имя"

[form.contact.email]
other = "Email"

[form.contact.phone]
other = "Телефон"

[form.contact.message_placeholder]
other = "Введите сообщение..."

[form.contact.submit]
other = "Отправить"
```

## en.toml

```toml
[form.contact.name]
other = "Name"

[form.contact.email]
other = "Email"

[form.contact.phone]
other = "Phone"

[form.contact.message_placeholder]
other = "Enter message..."

[form.contact.submit]
other = "Submit"
```

### Diagram

```
{{< diagram >}}
```

### Donate Form

Форма приёма пожервований.

## Syntax

```
{{< form-donate
wallet="[WALLET_YOOMONEY]"
paypal="[PAYPAL_EMAIL]"
patreon="[PATREON_USER]"
liberapay="[LIBERAPAY_USER]"
ko-fi="[KO-FI_USER]"
buymeacoffee="[BUYMEACOFFEE_USER]"
usd="[CARD_USD]"
eur="[CARD_EUR]"
rub="[CARD_RUB]"
btc="[WALLET_BTC]"
eth="[WALLET_ETH]"
xmr="[WALLET_XMR]" >}}
```

## ru.toml

```toml
[form.donate.targets]
other = "Назначение перевода..."

[form.donate.targets_help]
other = "Укажите назначение перевода."

[form.donate.sum_help]
other = "Укажите сумму."

[form.donate.card]
other = "Банковская карта"

[form.donate.yooMoney]
other = "ЮMoney"

[form.donate.mobile_phone]
other = "Мобильный телефон"

[form.donate.payment_type_help]
other = "Выберите способ перевода."

[form.donate.comment_placeholder]
other = "Введите комментарий (если имеется)..."

[form.donate.comment_help]
other = "Введите сопроводительный комментарий (не более 200 символов)."

[form.donate.name]
other = "ФИО"

[form.donate.name_help]
other = "Отметьте, если хотите указать ФИО отправителя."

[form.donate.email]
other = "E-mail"

[form.donate.email_help]
other = "Отметьте, если хотите указать электронную почту отправителя."

[form.donate.phone]
other = "Телефон"

[form.donate.phone_help]
other = "Отметьте, если хотите указать телефон отправителя."

[form.donate.address]
other = "Адрес"

[form.donate.address_help]
other = "Отметьте, если хотите указать адрес отправителя."

[form.donate.paypal]
other = "PayPal"

[form.donate.patreon]
other = "Patreon"

[form.donate.liberapay]
other = "Liberapay"

[form.donate.kofi]
other = "Ko-fi"

[form.donate.buymeacoffee]
other = "Buy Me a Coffee"

[form.donate.submit]
other = "Перевести"

[form.donate.btc]
other = "BTC"

[form.donate.eth]
other = "ETH"

[form.donate.xmr]
other = "XMR"

[form.donate.cards]
other = "Банковские карты"

[form.donate.crypto]
other = "Crypto"

[form.donate.services]
other = "Сервисы"
```

## en.toml

```toml
[form.donate.targets]
other = "Target transfer..."

[form.donate.targets_help]
other = "Enter target transfer."

[form.donate.sum_help]
other = "Set amount."

[form.donate.card]
other = "Bank Card"

[form.donate.yooMoney]
other = "YooMoney"

[form.donate.mobile_phone]
other = "Mobile Phone"

[form.donate.payment_type_help]
other = "Select a transfer method."

[form.donate.comment_placeholder]
other = "Enter a comment (if available)..."

[form.donate.comment_help]
other = "Enter an accompanying comment (max 200 characters)."

[form.donate.name]
other = "Name"

[form.donate.name_help]
other = "Check if you want to specify name of sender."

[form.donate.email]
other = "E-mail"

[form.donate.email_help]
other = "Check if you want to specify sender's e-mail."

[form.donate.phone]
other = "Phone"

[form.donate.phone_help]
other = "Check if you want to specify sender's phone number."

[form.donate.address]
other = "Address"

[form.donate.address_help]
other = "Check if you want to specify sender address."

[form.donate.paypal]
other = "PayPal"

[form.donate.patreon]
other = "Patreon"

[form.donate.liberapay]
other = "Liberapay"

[form.donate.kofi]
other = "Ko-fi"

[form.donate.buymeacoffee]
other = "Buy Me a Coffee"

[form.donate.submit]
other = "Transfer"

[form.donate.btc]
other = "BTC"

[form.donate.eth]
other = "ETH"

[form.donate.xmr]
other = "XMR"

[form.donate.cards]
other = "Bank Cards"

[form.donate.crypto]
other = "Crypto"

[form.donate.services]
other = "Services"
```

### EMOJI

```
{{< emoji "[ID]" "[SIZE]" >}}
```

### Gist

```
{{< gist "spf13" "7896402" >}}
```

```
{{< gist "spf13" "7896402" "img.html" >}}
```

### Icon

```
{{< icon "[PACK]" "[ICON]" >}}
```

#### PACK

- `fas`
- `far`
- `fal`
- `fad`
- `fab`

#### ICON

- `camera`
- ...

### Imgur

```
{{< imgur id="[ID]" size="[SIZE]" caption="[CAPTION]" align="[ALIGN]" >}}
```

#### ID

- `12345`

#### SIZE

- `s` - Small Square (90x90)
- `b` - Big Square (160x160)
- `t` - Small Thumbnail (160x160)
- `m` - Medium Thumbnail (320x320)
- `l` - Large Thumbnail (640x640)
- `h` - Huge Thumbnail (1024x1024)
- [more](https://api.imgur.com/models/image)

#### CAPTION

- `Lorem ipsum dolor sit amet, consectetur adipiscing elit.`

#### ALIGN

- `start`
- `end`
- `center`

### Instagram

```
{{< instagram "BWNjjyYFxVx" >}}
```

```
{{< instagram "BWNjjyYFxVx" "hidecaption" >}}
```

### Key

```
{{< key "[KEY]" >}}
```

#### KEY

- `CTRL`
- `ALT`
- `DEL`

### Map

```
{{< map [LAT] [LON] [ZOOM] [MLAT] [MLON] [MTXT] >}}
```

#### LAT

-

#### LON

-

#### ZOOM

-

#### MLAT

-

#### MLON

-

#### MTXT

-

### Mark

```
{{< mark "[TEXT]" >}}
```

### Mention

```
{{< mention "[USER]" >}}
```

### Progress

```
{{< progress "[SIZE]" "[TYPE]" >}}
```

#### SIZE

- `0` - `100`

#### TYPE

- `success`
- `info`
- `warning`
- `danger`

### Requisites

```
{{< requisites "[URL.JSON]" "[TYPE]" >}}
```

### Spoiler

```
{{< spoiler >}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis id neque a dolor ornare porttitor. Maecenas id est magna. Vivamus ut urna orci. Suspendisse quam lacus, volutpat vitae lectus quis, malesuada tempus magna. Ut cursus vel quam sit amet condimentum. Nam at dignissim dolor. Cras egestas lectus in odio auctor.
{{< /spoiler >}}
```

```
{{< spoiler title="[TITLE]" type="[TYPE]" >}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis id neque a dolor ornare porttitor. Maecenas id est magna. Vivamus ut urna orci. Suspendisse quam lacus, volutpat vitae lectus quis, malesuada tempus magna. Ut cursus vel quam sit amet condimentum. Nam at dignissim dolor. Cras egestas lectus in odio auctor.
{{< /spoiler >}}
```

#### TITLE

- `Lorem ipsum dolor sit amet, consectetur adipiscing elit.`

#### TYPE

- `primary`
- `secondary`
- `success`
- `danger`
- `warning`
- `info`
- `light`
- `dark`
- `link`

### Tags

```
{{< tags >}}
```

### Tweet

```
{{< tweet "877500564405444608" >}}
```

### Vimeo

```
{{< vimeo "146022717" >}}
```

### VK Users

```
{{< vk-users "[USER_ID_01],[USER_ID_02],[USER_ID_02]" >}}
```

Создать приложение, платформа **Сайт**.

```
https://oauth.vk.com/authorize?client_id=[ID]&display=page&redirect_uri=https://oauth.vk.com/blank.html&scope=offline&response_type=token&v=5.52
```

### YouTube

```
{{< youtube "w7Ft2ymGmfc" >}}
```

```
{{< youtube id="w7Ft2ymGmfc" autoplay="true" >}}
```

```
{{< youtube id="w7Ft2ymGmfc" title="A New Hugo Site in Under Two Minutes" >}}
```
