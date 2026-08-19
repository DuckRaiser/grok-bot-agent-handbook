# Playbook：找房扫盘

Schedule 配方：先改数字和城市，交给一个**只做找房**的 bot。对外问照片、议价，交给 Voice / Outbound，不要让找房 bot 学你的口吻。

配套：[06 变成你不在也跑的 routine](../docs/06-routines.md) · [07 雇专家](../docs/07-hire-specialists.md)

```
I want you to do sweeps every 6 hours of new housing that works for me.
I'm open to renting or buying.

Check Redfin, Zillow, StreetEasy (if they have SF housing),
and a few other sites. Suggest directories if needed.
Use the map image I provided as the general area I want to live in,
not as an exact pin.

Requirements:
- rent <4.5k (good value; 1 bedroom and up)
- purchase <1.3M
- HOA fees CANNOT exceed 500 dollars
- prefer not to exceed 450k per bedroom
- big windows, light from outside
- as many bathrooms as bedrooms
- pet friendly (I have a dog)

Send me a short report each sweep: address, price, why it fits,
what you could not verify. Do not invent listings.
If a site throws a CAPTCHA, 2FA, or payment wall: stop, screenshot, hand me the desktop.

Never submit an application, never pay, never message a listing
unless I say so. Draft outreach for Voice / Outbound; do not send it yourself.
```

## 改之前只动这些

- 城市和站点
- 租金 / 总价 / HOA / 每间房价
- 宠物、卧室、光照——写成可核对的硬条件，不要写「舒服就行」
- 发送权仍留给另一个职位或 Auto-review
