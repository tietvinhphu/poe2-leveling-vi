# Hướng dẫn PoE2 (Tiếng Việt) — Leveling Campaign, Endgame & Crafting

Bản dịch tiếng Việt của hướng dẫn **Path of Exile 2** tương tác, miễn phí, gồm leveling campaign (Act I–IV và các Interlude), lộ trình Endgame Atlas và Crafting Codex.

> **Đây là bản dịch.** Nội dung và mã nguồn gốc do **[domistae](https://github.com/domistae)** viết, tại [github.com/domistae/poe2-leveling](https://github.com/domistae/poe2-leveling) (trang gốc: [domistae.github.io/poe2-leveling](https://domistae.github.io/poe2-leveling/)), phát hành theo giấy phép MIT. Bản tiếng Việt này không do tác giả gốc xác nhận hay bảo trợ. Mọi sai sót trong bản dịch là của bản dịch, không phải của tác giả gốc.

**Trang web:** [tietvinhphu.github.io/poe2-leveling-vi](https://tietvinhphu.github.io/poe2-leveling-vi/)
**Patch mục tiêu:** PoE2 patch 0.5.5 (Forbidden Rites), theo bản gốc tại thời điểm dịch. Hướng dẫn luôn bám league đang chạy mới nhất và **không dành riêng cho Standard**.

## Trạng thái dịch

| Trang | Tiếng Việt |
| --- | --- |
| Trang chủ, hub Leveling, Act I, II, III, IV, Interlude, League (Conquerors of Wraeclast) | Đã dịch |
| Endgame (`poe2_endgame_guide.html`) | Chưa dịch, vẫn là tiếng Anh |
| Crafting Codex (`poe2_crafting_codex.html`) | Chưa dịch, vẫn là tiếng Anh |

## Quy ước dịch

PoE2 hiện chưa có client tiếng Việt, nên người chơi thấy toàn bộ tên trong game bằng tiếng Anh. Vì vậy bản dịch **giữ nguyên tiếng Anh** cho tên riêng và thuật ngữ in-game để bạn đối chiếu được với màn hình: tên zone, boss, NPC, vật phẩm, currency, skill gem, ascendancy, waypoint, passive tree, Spirit, Skill Points, Charm, Tribute, và các nhãn như `WAYPOINT`, `TOWN`, `Lvl`. Phần lời hướng dẫn, mô tả, mẹo và giao diện trang được dịch sang tiếng Việt. Từ "Opt" (optional) được dịch thành "Tùy chọn". Hướng la bàn trong phần Interlude dùng viết tắt tiếng Việt (B, N, Đ, T, ĐB, ĐN, TB).

## Tính năng

- ✓ **Checklist theo dõi tiến độ.** Bấm vào một dòng để đánh dấu hoàn thành (các trang campaign).
- 💾 **Tự lưu.** Tiến độ lưu trong localStorage của trình duyệt.
- 🧭 **Thanh điều hướng.** Chuyển nhanh giữa Leveling, Endgame và Crafting; tab Act / Interlude trên các trang campaign.
- 🎯 **Phần thưởng vĩnh viễn.** Mọi skill point, spirit và mở khóa đều được làm nổi bật.
- ⚡ **Lộ trình tối ưu.** Định tuyến waypoint hiệu quả, có chế độ "Chạy rút gọn".
- 🌓 **Giao diện sáng / tối.** Mặc định là tối.
- 📱 **Dùng được trên điện thoại.** Bố cục thanh bên co giãn.

## Cấu trúc file

```
index.html                   Trang chủ — hub Leveling / Endgame / Crafting
poe2_leveling_guide.html     Hub Leveling — Act I–IV + Interlude
poe2_act1_guide.html         Act I:   Clearfell → Ogham Manor
poe2_act2_guide.html         Act II:  Vastiri Desert → Dreadnought
poe2_act3_guide.html         Act III: Utzaal → Ziggurat
poe2_act4_guide.html         Act IV:  Keth → Nightmare of the King
poe2_interludes_guide.html   Act 5.1–5.3 (Interlude sau campaign)
poe2_endgame_guide.html      Endgame / Atlas (chưa dịch)
poe2_league_guide.html       Hướng dẫn league: Conquerors of Wraeclast
poe2_crafting_codex.html     Crafting Codex (chưa dịch)
assets/                      CSS, JS và font tự host (xem CLAUDE.md)
img/                         Ảnh thẻ và ảnh xem trước mạng xã hội
```

Dự án chỉ gồm HTML, CSS và JS thuần, không có bước build. Có thể chạy một server tĩnh trong thư mục gốc, ví dụ `python3 -m http.server 8765`.

## Khác biệt so với bản gốc

- Toàn bộ nội dung các trang đã nêu ở bảng trên được dịch sang tiếng Việt, kể cả chuỗi trong JS (giao diện sáng/tối, hộp thoại đặt lại tiến độ, tooltip).
- **Đã gỡ Google Analytics** và banner cookie. Bản gốc tải Google Analytics bằng mã theo dõi của tác giả gốc; bản dịch không gửi lượt truy cập của bạn cho bất kỳ ai. Chính sách nội dung bảo mật (CSP) cũng được siết lại tương ứng.
- Các liên kết trỏ về repo và trang web của bản dịch này; phần ghi công trong mỗi file vẫn giữ nguyên tác giả gốc.

## Nguồn và miễn trừ

Hướng dẫn gốc là **bản tóm tắt do cộng đồng viết**, tổng hợp từ chính game, dữ liệu cộng đồng như PoE2DB, các trang hướng dẫn (Maxroll, Mobalytics, Vulkk), thông báo và buổi stream chính thức của PoE2, và các buổi trình diễn craft của streamer. Bản gốc có AI hỗ trợ; các nguồn đôi khi mâu thuẫn, game thay đổi mỗi patch, và dữ liệu cộng đồng thường chậm hơn hành vi thật trong game. **Hãy xem đây là tài liệu tra nhanh, không phải tài liệu chính thức.** Trước khi craft tốn kém hoặc rủi ro cao, hãy đối chiếu với PoE2DB và tooltip trong game.

Bản dịch có thể còn sai sót hoặc lỗi thời so với bản gốc. Nếu thấy lỗi dịch, hãy [mở một issue](https://github.com/tietvinhphu/poe2-leveling-vi/issues/new). Nếu lỗi nằm ở nội dung gốc, hãy báo cho [repo gốc](https://github.com/domistae/poe2-leveling/issues/new).

## Giấy phép và ghi công

Mã nguồn và nội dung gốc được phát hành theo **Giấy phép MIT**, xem [LICENSE](LICENSE). Bản dịch này giữ nguyên thông báo bản quyền `Copyright (c) 2026 domistae` và văn bản giấy phép MIT, đồng thời ghi công nguồn gốc: [github.com/domistae/poe2-leveling](https://github.com/domistae/poe2-leveling). Nếu bạn dùng lại bản dịch này, hãy giữ nguyên các thông báo đó.

## Tuyên bố miễn trừ

Đây là trang fan miễn phí, không chính thức. Không liên kết, không được bảo trợ hay xác nhận bởi Grinding Gear Games. Path of Exile và Path of Exile 2 thuộc bản quyền © Grinding Gear Games. Mọi nhãn hiệu, tên sản phẩm, ảnh chụp màn hình, thuật ngữ và nội dung game thuộc về chủ sở hữu tương ứng.

Nội dung được chia sẻ nguyên trạng, không kèm bất kỳ bảo đảm nào. Nội dung có thể chưa đầy đủ, lỗi thời hoặc sai. Không chịu trách nhiệm về các quyết định trong game dựa trên tài liệu này. Hãy tự cân nhắc và kiểm chứng bằng tooltip trong game và PoE2DB.
