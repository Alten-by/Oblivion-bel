# Глосарый (en → bel) для перакладу Oblivion Remastered

Крыніцы: `skyrim` — беларускі пераклад Skyrim (тыя ж тэрміны ES); `custom` —
ужо зацверджаны чалавекам пераклад у гэтым праекце; `выбар` — прынята
падчас гэтай працы (няма гатовага ўзору), бліжэй да en.

Гэта жывы дакумент: падчас Кроку 3-4 сюды дадаюцца новыя тэрміны, якія
паўтараюцца больш за адзін раз.

## Стыль (назіранні з ~2100 ужо запоўненых `custom`)

- З 2106 запоўненых запісаў: 1290 (61%) супадаюць з `bel` дакладна, 268
  (13%) — з `bel_alt`, 550 (26%) напісаны нанова. **Пры сумневе `bel`
  часцей бліжэй да прынятага стылю, чым `bel_alt`**, але кожны запіс трэба
  правяраць асобна — `bel_alt` можа быць лепшы для канкрэтнага выпадку.
- Рэгістр: толькі першае слова і ўласныя назвы з вялікай літары
  (`Трансцэндэнтны сігільскі камень`, не `Трансцэндэнтны Сігільскі Камень`),
  нават калі ў `en` кожнае слова з вялікай (Title Case).
  Выключэнне: назвы, дзе кожнае слова - уласны назоўнік (`Гільдыя Байцоў
  Скінграда` як частка ўласнай назвы канкрэтнай гільдыі).
- «Guard»/«Watch» перакладаецца як **«стражнік»** для афіцыйнай варты
  (гарадской, імператарскай, палацавай: `Imperial Watch` → `Імперскі
  стражнік`, `Palace Guard` → `Палацавы стражнік`), і як **«ахоўнік»**
  для прыватнай/кампанейскай аховы (`Blackwood Company Guard` → `Ахоўнік
  кампаніі "Чорны лес"`).
- Назвы гарадоў/НПС карэктуюцца пад беларускае «дзеканне»/«цеканне»:
  `Cheydinhal` → `Чэйдзінхол` (не «Чэйдынхол»).
  Правярай назвы месцаў у glossary раздзеле «Правінцыя Cyrodiil» ніжэй.
  Двукоссі — простыя `"..."` (як ужо ва ўсіх existing `custom`), не «...».
- ICU `|plural(...)`/`|ordinal(...)`: сінтаксіс (`plural`, `ordinal`,
  `one=`, `few=`, `many=`, `other=`) заўсёды лацінкай, гэта не тэкст для
  перакладу. Значэнні пасля `=` — перакладаюцца/дадаюцца формы `one, few,
  many, other` нават калі ў `en` толькі `one, other`.
- **Увага, вядомая памылка чарнавікоў**: у `bel`/`bel_alt` (і зрэдку ў
  ўжо гатовым `custom`) сустракаецца пашкоджаны тэг `<cf>` замест `<lf>`
  (перавод радка). `<cf>` НІКОЛІ не сустракаецца ў `en` — калі бачыш яго ў
  чарнавіку, гэта заўсёды памылка, бяры `<lf>` з `en`. Таксама сустракаюцца
  тэгі з лішнім прабелам (`< RT_BlueMed>` замест `<RT_BlueMed>`) — заўсёды
  капіюй тэг символ-у-символ з `en`.

## Устойлівыя канструкцыі (Resist/Weakness/Magicka і інш.)

Пацверджана шматлікімі ўжо гатовымі `custom` у гэтым праекце (НЕ Skyrim -
тут свая, іншая за Skyrim, усталяваная тэрміналогія):

| Канструкцыя | Пераклад | Прыклад |
|---|---|---|
| `X Resistance` / `Resist X` (з мадыфікатарам-расай/рангам) | `Супраціўленне X [мадыфікатар, родны]` | "Churl Resist Magic" -> "Супраціўленне магіі Чурла" |
| `Resist X` (без мадыфікатара, кароткая назва эфекту) | `Супраціў X` | "Resist Magic" -> "Супраціў магіі" |
| `[Раса] X Resistance/Immunity` (агульная расавая рыса) | `[Імунітэт/Супраціў] [расы, родны склон мн.] [чаму]` | "Nord Frost Immunity" -> "Імунітэт нордаў да холаду" |
| `Weakness to X` | `Уразлівасць да X` | НЕ "слабасць" |
| `Magicka` (рэсурс, не паняцце "магія" увогуле) | `магія` | скайрымскі пераклад таксама выкарыстоўвае "магія" |
| `Rending Halls` | `Палацы разлукі` | ужо гатовы custom |

Гл. таксама раздзел «Аўтаматычна вывераныя тэрміны» ніжэй для іншых
устойлівых спалучэнняў.

## Увага пры выбары bel/bel_alt (знойдзена ў порцыі 1)

- Гарадскія назвы (Анвіл, Бравіл і інш.) у чарнавіках часам пакінуты
  лацінкай ("Anvil") або няправільна ПЕРАКЛАДЗЕНЫ як агульны назоўнік
  ("Накавальня" замест "Анвіл") - заўсёды правяраць і выпраўляць на
  транслітараваную ўласную назву з glossary.md.
- "Арэна" (The Arena, Imperial City) - уласная назва, заўсёды з вялікай
  літары нават у родным/месным склоне: Арэны, Арэне, Арэну.
- Асабістыя імёны NPC часта разыходзяцца паміж bel/bel_alt (транслітарацыя
  varies) - калі яны паўтараюцца ў некалькіх запісах (напр. "Branwen and
  Saliith"), трэба выбраць АДЗІН варыянт і трымацца яго ва ўсіх запісах.

## Дадаткова (порцыя 2)

- Лацінскі дыфтонг "au" у імёнах -> "аў" (не "ау"): "Baurus" -> "Баўрус",
  "Bawn" -> "Баўн" (адпавядае агульнаму правілу перадачы "au" у беларускай).
- "Bound X" (закляцце школы Выклікання, часовая зброя/браня) -> "Прызваны/-ая/-ыя X"
  (заклятая рэч "прызываецца" адпаведна школе магіі). АЛЕ "Bound Order
  Weapon" (эфект ад дэйдра Парадку) -> "Звязаная зброя Ордэна" - ужо
  замацавана ў same_bel_belalt_case_insensitive.json, не блытаць.
- "Atronach" -> "атранах" (не "атронах"/"атранах" - глядзі ўзор у ужо
  гатовым custom "Агонь атранаха"/"Мароз атранаха").
- "Blackwood Company" (арганізацыя) -> заўсёды `кампанія "Чорны лес"`
  (з двукоссямі, ужо замацавана ў custom). "Blackwood" як геаграфічная
  вобласць (не арганізацыя) -> кампактнае "Чарналес".
- "Blades" (арганізацыя) -> "Клінкі" (скланяецца: Клінкоў, Клінкам).
  НЕ блытаць з "Blademaster" (агульны тытул майстра мяча, не абавязкова
  звязаны з арганізацыяй Клінкоў) -> "Майстар мяча".
- "Belisarius" -> "Белісарый" (стандартная беларуская форма гістарычнага
  імя, не "Белізарыус").
- Тэхнічныя ідэнтыфікатары тыпу "BarterBuyItem", "BladesTalk1" (склееныя
  ангельскія словы без прабелаў) - калі яны ўсё ж такі маюць сэнс для
  гульца (напр. вынік мінііgры "Пераканаць" AdmireFail/BOAST_HATE),
  перакладаем натуральнай фразай. Чыста код/сцэнарныя ідэнтыфікатары без
  моўнага сэнсу (напр. "SE03GrommokChamberTwoManEnd03") капіюем як ёсць.

## Дадаткова (порцыя 3)

- Кніжныя серыі ES (Barenziah, 2920, Feyfolken і інш.): нумар тома
  перадаецца як "т. N" (з прабелам), не "тN"/"vN"; рымскія лічбы (I, II,
  III) у назвах застаюцца як у en.
- "Undercroft" (склеп пад капліцай) -> "Крыпта" (не "склеп"/"падзямелле").
- "Manor" (сядзіба лорда/графа) -> "сядзіба", калі агульны тэрмін;
  канкрэтны асабняк у горадзе -> "асабняк".
- "NQD"/"CG" (тэхнічныя прэфіксы: NQD = "no quest dialogue"?, CG =
  Character Generation) застаюцца лацінкай у тэхнічных ідэнтыфікатарах
  кшталту "Адказы NQD Брумы" - гэта чакана, не памылка.

## Дадаткова (порцыя 4)

- **Chorrol -> Корал** (не "Чорал"! пацверджана шматлікімі ўжо гатовымі
  custom, гл. аўтаматычную табліцу ніжэй). Родны склон - "Корала".
- Cheydinhal -> "Чэйдзінхол" застаецца асноўным напісаннем (гл. порцыю 1);
  у гэтай порцыі знойдзена шмат чарнавікоў з "Чэйдынхол"/"Чэйдынхал" -
  заўсёды выпраўляць на "Чэйдзінхол"/"Чэйдзінхола".
- "Clavicus Vile" -> "Клавікус Подлы" (глядзі раздзел «Даэдрычныя
  прынцы») - у гэтай порцыі чарнавікі давалі "Вайл", выпраўлена.
- "Chainmail X" -> "Кольчужны X" (не "Ланцужны").
- "Greaves" (без кантэксту "of X") -> заўсёды "Понажы".

## Дадаткова (порцыя 5) - усе даэдрычныя святыні

Устаноўлена: "Shrine of X" -> **"Святыня X"** (не "Свяцілішча") ва ўсіх
квэстах даэдрычных прынцаў. Выпраўленыя напісанні (чарнавікі часта
блыталі): Hermaeus Mora -> **Хермэўс Мора**; Hircine -> **Хірсін**;
Nocturnal -> **Накцюрнал** (НЕ перакладаць як "Начны" - гэта ўласнае
імя!); Peryite -> **Перыайт**; Vaermina -> **Вэрміна**; Sanguine ->
**Сангвін** (НЕ "Крывавы"); Sheogorath -> **Шэагорат** (родны
"Шэагората"). "Corruption" (Skull of Corruption) -> "Раскладанне".
"Greaves" (без кантэксту) -> заўсёды "Понажы", "Gauntlets" -> "Пальчаткі".

## Дадаткова (порцыя 6)

- **Увага да канцавой пунктуацыі**: шматлікія кароткія дыялогавыя рэплікі
  тыпу "I prefer Bows"/"Nevermind"/"I'd like a weapon" НЕ маюць кропкі ў
  `en` - не дадаваць яе і ў `custom` (validate.py гэта ловіць).
- Mehrunes Dagon -> заўсёды "Мехрунс" (родны "Мехрунса"), не "Мерунес".
- "Battle-Axe/Warhammer/Mace of Cataclysm/Order" -> "Сякера/Баявы
  молат/Булава Катаклізму/Парадку" (без "баявая" перад Сякера, per
  skyrim-прынцып для War Axe).
- "Drothmeri X" -> заўсёды "Дротмерскі X" (прыметнік).
- Chest/Gauntlets/Greaves у DL9/DLC06 блоках - шмат чарнавікоў з памылкай
  "Пячаткі" замест "Пальчаткі" (аднолькавы паўтаральны глюк) - заўсёды
  правяраць.

## Дадаткова (порцыя 7) - вялікі блок DLC-заклёнаў/тамоў

- "X Tome" (кніга заклёну) -> `Том "X"` (двукоссі, як цытата назвы
  заклёну ўнутры). Базавае імя заклёну заўсёды аднолькавае паміж версіяй
  "X" (сам заклён) і "X Tome" (том з заклёнам).
- Узроўні ўзмацнення: Minor -> Малое, Major -> Выдатнае, Greater ->
  Вышэйшае/Вышэйшы, Superior -> Найвышэйшае.
- "Bolt"-заклёны (Frost/Electrifying/...) -> "болт" (устойлівая ІТ-магічная
  лексіка), "Burst" -> "выбух", "Blast" -> "зарад" (адрозніваць!), "Touch"
  -> заўсёды "дотык".
- "Battlehorn" паўсюль -> "Баявы Рог" (родны склон "Баявога Рога").
- Дракон у кантэксце ўласна беларускай міфалогіі -> "цмок" (не "дракон"),
  напр. "Dragon Breath" -> "Дыханне цмока".
- Castellan (тытул) -> "Каштэлян" (гістарычны беларускі тэрмін, не
  "кастэлян").

## Дадаткова (порцыя 8) - працяг тамоў DLC + блок "Dark0X" (Цёмнае Брацтва)

- Атрыбут Personality у тытулах тамоў ("Fortify/Restore Personality Tome")
  -> "асобы" (не "абаяння"), для адпаведнасці ўжо ўсталяванаму
  Personality -> Асоба.
- Тэхнічныя ідэнтыфікатары ўнутры `en` (напр. "Dark02PirateConvo",
  "Dark04 Prison Guard") пераносяцца ў `custom` як ёсць (лацінка), калі
  яны ёсць у самім `en` -- гэта не памылка, гл. REVIEW.md/validate.py.
- Цёмнае Брацтва -> "Цёмнае Брацтва" (з вялікай літары, уласная назва
  арганізацыі). Sithis -> "Сіціс". The Night Mother -> "Маці Ночы".
- Daedra (як народ/раса) -> "дэйдра" (нескланяльнае, як у skyrim-крыніцы),
  Daedric (прыметнік) -> "дэйдрычны".

## Дадаткова (порцыя 9) - блок квэстаў Цёмнага Брацтва Dark06-Dark19

- Sithis -> "Сіціс". The Night Mother -> "Маці Ночы". The Black Hand ->
  "Чорная Рука". Listener -> "Слухач". Speaker (тытул) -> "Прамоўца".
- Рангі Цёмнага Брацтва: Slayer -> Знішчальнік, Eliminator -> Ліквідатар,
  Silencer -> Душыцель, Speaker -> Прамоўца (адзін і той жа тытул для
  муж./жан. формы, бо ў лоры гэта пасада, не асоба).
- Shadowmere (конь) -> "Ценявая Грыва".
- Тэхнічныя ідэнтыфікатары кшталту "DarkXXTalk"/"DarkXXConvo" без
  прасторавых слоў у `en` -> перакладаем апісальна + пакідаем raw ID
  побач (напр. "Размова са статуяй 1 Dark19StatueTalk1"), калі ва ўжо
  запоўненых `custom` няма іншай усталяванай канвенцыі.

## Дадаткова (порцыя 10) - Dremora рангі і зброя, хваробы, Doomstones

- Рангі дрэмора (Dremora Faction): Churl -> Керл, Caitiff -> Кайтыф,
  Kynval -> Кінвал, Kynreeve -> Кінрыў, Kynmarcher -> Кінмаршэр,
  Markynaz -> Маркіназ, Valkynaz -> Валкіназ. Агульны народ дрэмора -
  "Kyn" -> "Кін". Ва ўсіх складаных найменнях брані/зброі рангі
  ставяцца праз злучок: "дрэмора-кайтыфа", "дрэмора-кінрыў" і г.д.
  (родны склон для прадметаў, назоўны для істот).
  Dwarven (зброя/браня) -> "Двэмерскі" (ад Dwemer, не "дварфійскі").
- Хваробы (Diseases) перакладаюцца апісальна па сімптомах, а не
  літаральна: Rockjoint -> Каменная падагра, Witbane -> Разрэджванне
  мозгу, Serpiginous Dementia -> Змяіная дэменцыя.
- Doomstones (камяні знакаў Задыяка) -> "Камень + назва знака" (Камень
  Лэдзі, Камень Лорда, Камень Змяі і г.д.), спецэфекты каменя маюць
  уласныя паэтычныя назвы (Sands of Resolve -> Пясок Рашучасці).

## Дадаткова (порцыя 11) - вялікі блок зачараванай зброі/брані (Ench*)

- Схема "X of Y" (зачараваная зброя/браня) -> "<прадмет назоўнага роду>
  <назва эфекту ў родным склоне>", без арт. "of": "Battle-Axe of Winter"
  -> "Сякера зімы", "Cuirass of Fortitude" -> "Кіраса стойкасці".
  "Battle-Axe"/"War Axe" абодва -> "Сякера" (гіст. беларускі тэрмін для
  сякеры бою), не "топар"/"баявая сякера" паўтарана без патрэбы.
  "Warhammer"/"War Hammer" -> "Баявы молат".
  "Fortitude/Endurance/Health" эфекты часта перадаюцца пераносна
  (Salubrious -> Аздараўляльная, Stalwart -> Умацоўваючая), а не
  літаральна.
- Уласныя назвы персанажаў/убораў у en застаюцца лацінкай толькі калі
  гэта чыста тэхнічны запіс (ru таксама лацінкай); калі ёсць паралельны
  варыянт з транслітарацыяй (Uriel/Martin -> Урыэль/Марцін), выбіраем
  транслітараваны варыянт, каб пазбегнуць лацінкі ў custom.

## Дадаткова (порцыя 14) - форты, Frostcrag Spire, гобліны

- Frostcrag (Spire) -> транслітаравана "Фросткраг" паўсюль (не
  перакладаецца як "Ледзяны Пік"), для аднастайнасці з большасцю ўжо
  запоўненых `custom`.
- Fort-назвы: калі гэта чыста апісальная англійская фраза (Fort Grief,
  Fort Blueblood) -> перакладаем цалкам ("Форт Гора", "Форт Блакітнай
  Крыві"); калі ўласнае імя -- транслітаруем (Fort Entius -> Форт
  Энцый). Пры разыходжаннях паміж запісамі аднаго форта -- прыводзім да
  адзінага варыянту.
- Francois Motierre -> "Франсуа Моцьер" (склонавая форма "Моцьера"),
  замацавана ўжо ў квэстах Цёмнага Брацтва (порцыя 9).
- Гобліны: назвы плямёнаў/варт перакладаюцца (Bloody Hand -> Крывавыя
  рукі, Rock Biter -> Скалягрызы, Skull Breaker -> Знішчальнікі
  чарапоў), правадыр -> "правадыр".

## Дадаткова (порцыя 15) - "Goodbye"/"Greeting" рэплікі, коні

- "GoodbyeX"/"GreetingX" тэхнічныя ключы, дзе X -- імя боства/NPC/месца:
  заўсёды транслітараваць уласнае імя (Akatosh->Акатош, Kvatch->Кватч,
  Mara->Мара, Talos->Талас), ніколі не пакідаць лацінкай, нават калі
  чарнавік bel так зрабіў.
  Divine (як тытул "the Divines") -> "Боства"/"Боствы".
  Stendarr -> "Стэндар" (не "Стэндарр", як у Skyrim -- у гэтай мадэлі
  ужыта аднаапорнае "р").
- Коні (Horse): Bay Horse -> Чалая кабыла, Chestnut Horse -> Гнядая
  кабыла (устал. праз бел, нягледзячы на тое, што "Chestnut/Bay" —
  масці буйна; заўважце розніцу з "Armored Chestnut" — "Каштанавы конь"
  у зачараваных версіях).

## Расы (Races)

| en | bel | крыніца |
|---|---|---|
| Argonian | Аргоніянец | skyrim |
| Altmer / High Elf | Высокі эльф | skyrim |
| Bosmer / Wood Elf | Лясны эльф | skyrim |
| Breton | Брэтон | skyrim |
| Dunmer / Dark Elf | Цёмны эльф | skyrim |
| Imperial | Імперац | skyrim |
| Khajiit | Каджыт | skyrim/custom |
| Nord | Норд | skyrim |
| Orc / Orsimer | Орк | skyrim |
| Redguard | Рэдгард | skyrim |

## Даэдрычныя прынцы (Daedric Princes)

| en | bel | крыніца |
|---|---|---|
| Azura | Азура | skyrim |
| Boethiah | Баэція | skyrim |
| Clavicus Vile | Клавікус Подлы | skyrim |
| Hermaeus Mora | Хермэўс Мора | skyrim |
| Hircine | Хірсін | skyrim |
| Malacath | Малакат | skyrim |
| Mehrunes Dagon | Мехрунс Дагон | выбар |
| Mephala | Мефала | skyrim |
| Meridia | Мерыдыя | skyrim |
| Molag Bal | Молаг Бал | skyrim |
| Namira | Наміра | custom(bel) |
| Nocturnal | Накцюрнал | skyrim |
| Peryite | Перыайт | custom(bel) |
| Sanguine | Сангвін | skyrim |
| Sheogorath | Шэагорат | skyrim |
| Vaermina | Вэрміна | skyrim |
| Daedra / Daedric Prince | Даэдра / Даэдрычны прынц | выбар |
| Jyggalag | Джыгалаг | выбар |
| Umaril (the Unfeathered) | Умарыл (Абязвечаны) | выбар |

## Школы магіі (Schools of Magic)

| en | bel | крыніца |
|---|---|---|
| Alteration | Змяненне | skyrim |
| Conjuration | Выкліканне | skyrim |
| Destruction | Разбурэнне | skyrim/custom |
| Illusion | Ілюзія | skyrim/custom |
| Mysticism | Містыцызм | custom(bel) |
| Restoration | Аднаўленне | skyrim |

## Атрыбуты (Attributes)

| en | bel | крыніца |
|---|---|---|
| Strength | Сіла | выбар |
| Intelligence | Інтэлект | выбар |
| Willpower | Сіла волі | выбар |
| Agility | Спрыт | выбар |
| Speed | Хуткасць | выбар |
| Endurance | Вынослівасць | выбар |
| Personality | Асоба | выбар |
| Luck | Удача | выбар |

## Навыкі (Skills)

| en | bel | крыніца |
|---|---|---|
| Acrobatics | Акрабатыка | выбар |
| Alchemy | Алхімія | skyrim/custom |
| Armorer | Рамонт брані | выбар |
| Athletics | Атлетыка | выбар |
| Blade | Валоданне клінком | выбар |
| Block | Блакаванне | skyrim |
| Blunt | Валоданне тупой зброяй | выбар |
| Conjuration | Выкліканне | skyrim |
| Hand to Hand | Рукапашны бой | выбар |
| Heavy Armor | Цяжкая браня | выбар |
| Light Armor | Лёгкая браня | выбар |
| Lockpicking / Security | Узлом | skyrim |
| Marksman | Стральба з лука | skyrim |
| Mercantile | Гандаль | выбар |
| Mysticism | Містыцызм | custom(bel) |
| Sneak | Скрытнасць | skyrim |
| Speechcraft | Красамоўства | skyrim |
| Hand-to-Hand | Рукапашны бой | выбар |
| Pickpocket | Кішэнны крадзеж | skyrim |

## Правінцыя Cyrodiil / геаграфія

| en | bel | крыніца |
|---|---|---|
| Cyrodiil | Сіродзіл | custom(bel) |
| Tamriel | Тамрыэль | skyrim |
| Oblivion (план) | Аблівіён | custom (draft "Аблівіён"/"Аблівіан" - выбраны "-іён", натуральней для беларускай) |
| Nirn | Нірн | выбар |
| Mundus | Мундус | выбар |
| Skyrim | Скайрым | skyrim |
| Morrowind | Морравінд | выбар |
| Anvil | Анвіл | выбар |
| Bravil | Бравіл | custom |
| Bruma | Брума | custom |
| Cheydinhal | Чэйдзінхол | custom |
| Chorrol | Корал | custom (пацверджана шматлікімі ўжо гатовымі custom) |
| Kvatch | Кватч | выбар |
| Leyawiin | Леявін | выбар |
| Skingrad | Скінград | custom |
| Imperial City | Імперскі Горад | выбар |

## Фракцыі / арганізацыі

| en | bel | крыніца |
|---|---|---|
| Fighters Guild | Гільдыя байцоў | custom(bel) |
| Mages Guild | Гільдыя магаў | custom(bel) |
| Thieves Guild | Гільдыя злодзеяў | custom(bel) |
| Dark Brotherhood | Цёмнае Братэрства | custom(bel) |
| Blackwood Company | Кампанія "Чорны лес" | custom |
| Imperial Legion | Імперскі легіён | custom |
| Knights of the Nine | Рыцары Дзевяці | выбар |
| Mythic Dawn | Міфічны Світанак | custom |
| Blades | Клінкі | выбар |

## Зброя і браня (кампаненты назваў наборы Order/Cataclysm/Crusader)

| en | bel | крыніца |
|---|---|---|
| of Order | Парадку | custom |
| of Cataclysm | Катаклізму | выбар |
| of the Crusader | Крыжака | custom (пацверджана 25× у filled custom: "Пальчаткі/Понажы/... Крыжака") |
| Sword | Меч | выбар |
| Longsword | Доўгі меч | выбар |
| Claymore | Клеймара | выбар |
| Dagger | Кінжал | выбар |
| Mace | Булава | выбар |
| Warhammer | Баявы молат | выбар |
| Battle-Axe / Battleaxe / War Axe | Сякера | custom (skyrim: "Daedric War Axe"->"Сякера дэйдра" - без "баявая") |
| Bow | Лук | выбар |
| Arrow | Стрэла | выбар |
| Shield | Шчыт | custom |
| Helm / Helmet | Шлем | выбар |
| Cuirass | Кіраса | выбар |
| Greaves | Понажы | custom |
| Gauntlets | Наручы | skyrim |
| Boots | Боты | skyrim/custom |
| Robe | Мантыя | выбар |
| Amulet | Амулет | выбар |
| Ring | Пярсцёнак | custom(bel) |
| Sigil Stone | Сігільскі камень | custom |
| Daedric War Axe | Сякера дэйдра | skyrim |
| Dwarven (Dwemer) X | Дзвемерскі X | выбар (ІНФА: "Dwarven" у ES = раса Dwemer, НЕ літаральныя гномы; "Дварфійскі" - НЕПРАВІЛЬна) |
| Ebony X | Эбанітавы X | custom |
| Orcish X | Аркоўскі X | выбар |
| Arch-Mage | Арцымаг | выбар (беларускі прэфікс "арцы-" як у "арцыбіскуп", не "архі-") |

## Істоты (bestiary)

| en | bel | крыніца |
|---|---|---|
| Daedroth | Дэйдрот | custom |
| Dremora | Дрэмора | custom/skyrim |
| Clannfear | Кланфір | выбар |
| Goblin | Гоблін | выбар |
| Minotaur | Мінатаўр | выбар |
| Troll | Троль | skyrim |
| Ogre | Огр | выбар |
| Zombie | Зомбі | skyrim |
| Skeleton | Шкілет | выбар |
| Ghost | Прывід | выбар |
| Lich | Ліч | выбар |
| Necromancer | Некрамант | skyrim/custom |
| Vampire | Вампір | skyrim/custom |
| Werewolf | Ваўкалак | skyrim |
| Golden Saint | Залатая святая | skyrim |
| Dark Seducer | Цёмны спакуснік | skyrim |
| Scamp | Скамп | выбар |
| Xivilai | Ксівілай | выбар |
| Flame Atronach | Агнявы атранах | custom(узор: "Агонь атранаха") |
| Frost Atronach | Марозны атранах | custom(узор: "Мароз атранаха") |
| Storm Atronach | Штармавы атранах | выбар |
| Flesh Atronach | Плоцевы атранах | выбар |
| Grummite | Грамміт | custom |
| Sheep | Авечка | выбар |
| Deer | Алень | skyrim |
| Bandit | Бандыт | custom |
| Marauder | Мародзёр | выбар |
| Pirate | Пірат | skyrim |
| Adventurer | Авантурыст | custom |
| Apostle | Апостал | выбар |

## Прадметы інтэр'ера / кантэйнеры

| en | bel | крыніца |
|---|---|---|
| Chest | Куфар | custom |
| Crate | Скрыня | выбар |
| Small Crate | Малая скрыня | выбар |
| Barrel | Бочка | skyrim |
| Cupboard | Буфет | custom |
| Drawers | Камода | custom |
| Bench | Зэдлік | skyrim |
| Chair | Крэсла | skyrim |
| Stool | Услончык | выбар |
| Bed | Ложак | skyrim |
| Coffin | Труна | custom |
| Urn | Урна | custom |
| Door | Дзверы | custom |
| Wooden Door | Драўляныя дзверы | skyrim |
| Metal Gate | Металічная брама | выбар |
| Gate | Брама | custom |
| Push Button | Кнопка | выбар |
| Handbill | Улётка | выбар (дакладней за "аб'яву" - лісток-рэклама) |
| Jewelry Box | Скрынка для ўпрыгожванняў | выбар |
| Anvil | Кавадла | выбар |

## Аўтаматычна вывераныя тэрміны (частата ≥2, з `custom`/`skyrim`)

| en | bel | крыніца |
|---|---|---|
| Chest | Куфар | custom |
| Wooden Door | Драўляныя дзверы | skyrim |
| Door | Дзверы | custom |
| Imperial Watch | Імперскі стражнік | custom |
| Bed | Ложак | skyrim |
| Barrel | Бочка | skyrim |
| Cupboard | Буфет | custom |
| Dark Seducer | Цёмны Спакуснік | skyrim |
| Grummite Whelp | Юны граміт | custom |
| Drawers | Камода | custom |
| Bench | Зэдлік | skyrim |
| [Say nothing.] | [Нічога не казаць.] | custom |
| Priest of Order | Жрэц парадку | custom |
| Knight of Order | Рыцар Парадку | custom |
| Imperial Legion Soldier | Салдат Імперскага легіёна | custom |
| Chair | Крэсла | skyrim |
| Gate | Брама | custom |
| Transcendent Sigil Stone | Цудоўны сігільскі камень | custom |
| Subjacent Sigil Stone | Базісны сігільскі камень | custom |
| Latent Sigil Stone | Латэнтны сігільскі камень | custom |
| Descendent Sigil Stone | Першасны сігільскі камень | custom |
| Ascendent Sigil Stone | Дамінантны сігільскі камень | custom |
| Coffin | Труна | skyrim |
| Urn | Урна | skyrim |
| Oblivion Gate | Брама Аблівіана | custom |
| Golden Saint | Залаты Святы | skyrim |
| Palace Guard | Палацавы стражнік | custom |
| No. | Не. | skyrim |
| Sack | Мяшок | custom |
| Mythic Dawn Guard | Стражнік Міфічнага Світанку | custom |
| Bruma Guard | Стражнік Брумы | custom |
| Iron Gate | Жалезная брама | custom |
| Follow me. | Ідзі за мной. | skyrim |
| Necromancer | Некрамант | skyrim |
| Golden Saint Helmet | Шлем залатых святых | custom |
| Dark Seducer Helmet | Шлем цёмных спакуснікаў | custom |
| Cheydinhal Guard | Стражнік Чэйдзінхола | custom |
| Auroran | Аўрорыянец | custom |
| Skingrad Guard | Стражнік Скінграда | custom |
| Drothmeri Soldier | Дротмер-салдат | custom |
| Corrupted Clone | Сапсаваны клон | custom |
| Chorrol Guard | Стражнік Корала | custom |
| Zealot Neophyte | Зелот-неафіт | custom |
| Rat | Пацук | custom |
| Beggar | Жабрак | skyrim |
| Yes. | Так. | skyrim |
| Bravil Guard | Стражнік Бравіла | custom |
| Bandit | Бандыт | skyrim |
| Skeleton | Шкілет | custom |
| Imperial Legion Horse | Конь Імперскага легіёна | custom |
| Dummy cell | Пустая ячэйка | custom |
| Desk | Пісьмовы стол | custom |
| Old Wooden Door | Старыя драўляныя дзверы | skyrim |
| Hollowed Stump | Полы пень | custom |
| Golden Saint Guard | Залаты святы - страж | custom |
| Germinal Gnarl | Гермінальны гнарл | custom |
| Gatekeeper | Страж брамы | custom |
| Chime | Звон | custom |
| Ayleid Cask | Айлейдская бочка | custom |
| Dremora Kynval | Дрэмора-кінвал | custom |
| Conjurer | Выклікальнік | skyrim |
| Zombie | Зомбі | custom |
| Trap Door | Лаз | skyrim |
| Throne | Пасад | skyrim |
| Stone Door | Каменныя дзверы | custom |
| Shadowrend | Разарваная Цень | custom |
| Ring of Lordship | Пярсцёнак Улады | custom |
| Leyawiin City Watch | Вартавы Лейавіна | custom |
| Geared Batten | Механізм | custom |
| Assassin | Забойца | custom |
| Who are you? | Хто ты? | skyrim |
| Sigil Stone | Сігільскі камень | custom |
| Ogre | Огр | custom |
| Not yet. | Яшчэ не. | skyrim |
| Marauder | Марадзёр | skyrim |
| Golden Saint Armor | Даспехі залатых святых | custom |
| Gauntlets of the Crusader | Пальчаткі Крыжака | custom |
| Fortify Magicka | Павышэнне магіі | custom |
| Entropic Bolt | Страла энтрапіі | custom |
| Display Case | Вітрына | skyrim |
| Dark Seducer Armor | Даспехі цёмных спакуснікаў | custom |
| Wait here. | Чакай тут. | skyrim |
| Rockshatter | Скалалом | custom |
| Mythic Dawn Agent | Агент Міфічнага Світанку | custom |
| Mystic Venom | Містычны яд | skyrim |
| Greaves of the Crusader | Понажы Крыжака | custom |
| Greaves of Order | Понажы Парадку | custom |
| Gauntlets of Order | Наручы Парадку | custom |
| Gauntlets of Cataclysm | Рукавіцы Катаклізму | custom |
| Drothmeri Recruit | Дротмер-рэкрут | custom |
| Dremora Churl | Дрэмора-керл | custom |
| Cuirass of Order | Кіраса Парадку | custom |
| Counter | Стойка | custom |
| Sigillum Sanguis | Сігілум Сангвіс | custom |
| Shambles | Кавардак | custom |
| Scamp | Скамп | custom |
| Mythic Dawn Acolyte | Служыцель Міфічнага Світанку | custom |
| Mage | Чараўнік | skyrim |
| Dremora Markynaz | Дрэмора-маркіназ | custom |
| Dremora Caitiff | Дрэмора-кайтыф | custom |
| Crystal Staff | Крыштальны посаx | custom |
| Blood Price | Цана крыві | custom |
| Blind Moth Priest | Сляпы жрэц Матылька | custom |
| Bandit Ringleader | Верхавод бандытаў | custom |
| Ascended Immortal | Узнесены несмяротны | custom |
| Shopping List | Рэцэпт | custom |
| Pirate | Пірат | skyrim |
| Note | Запіска | custom |
| Never mind. | Забудзь. | custom |
| Dremora Valkynaz | Дрэмора-Валкіназ | skyrim |
| Dremora Kynreeve | Дрэмора-Кінрыў | skyrim |
| Daedroth | Дэйдрот | custom |
| Boethia's Chosen | Выбраны Боэціі | custom |
| Bandit Bowman | Бандыт-лучнік | custom |
| Adventurer | Авантурыст | custom |
| Troll | Троль | skyrim |
| Restore Health | Аднаўленне здароўя | skyrim |
| Rending Halls | Палацы разлукі | custom |
| Portal | Партал | skyrim |
| Planter | Вазон | skyrim |
| No, not yet. | Не, яшчэ не. | custom |
| Magic Resistance | Супраціўленне магіі | custom |
| Deer | Алень | skyrim |
| Daedric War Axe | Сякера дэйдра | skyrim |
| Corridors of Dark Salvation | Калідоры Чорнага выратавання | custom |
| Regeneration | Рэгенерацыя | custom |
| Necromancer Adept | Некрамант-адэпт | skyrim |
| Letter | Ліст | skyrim |
| Ladder | Драбіны | skyrim |
| I'm not ready yet. | Мне яшчэ трэба падрыхтавацца. | skyrim |
| Heal | Лячыць | skyrim |
| Guard | Вартавы | skyrim |
| Conjurer Adept | Выклікальнік-адэпт | skyrim |
| Chapel Hall | Хол капліцы | custom |
| Bound Dagger | Прызваны кінжал | custom |
| Blade of Woe | Клінок Журбы | skyrim |
| Basket | Кошык | skyrim |
| Weakness to Fire | Уразлівасць да агню | skyrim |
| Water Healing | Лячэнне вадой | custom |
| Prisoner | Вязень | skyrim |
| Nerveshatter | Нерватраўнік | skyrim |
| I'm not interested. | Мне нецікава. | skyrim |
| Golden Saint Warrior | Залаты Святы-ваяр | skyrim |
| Golden Saint Shield | Шчыт Залатога Святога | skyrim |
| Dark Seducer Warrior | Цёмны Спакуснік-ваяр | skyrim |
| Dark Seducer Shield | Шчыт Цёмнага Спакусніка | skyrim |
| Dark Seducer Archer | Цёмны Спакуснік-лучнік | skyrim |
| Yes, I'm ready. | Так, можна пачынаць. | skyrim |
| YOU ARE USING WRONG GAMESETTING | ВЫ КАРЫСТАЕЦЕСЯ ПАМЫЛКОВЫМІ НАЛАДАМІ ГУЛЬНІ | custom |
| War Gate | Брама вайны | custom |
| Vampirism | Вампірызм | skyrim |
| Sword of Jyggalag | Меч Джыгалага | skyrim |
| Restore Magicka | Аднаўленне магіі | skyrim |
| Not right now. | Не зараз. | skyrim |
| Mercenary | Найміт | skyrim |
| Grand Soul Gem | Вялікі камень душ | skyrim |
| Ghost | Здань | skyrim |
| Dog | Сабака | skyrim |
| Chillrend | Ахаладжальнік | skyrim |
| Champion | Заступнік | skyrim |
| Absorb Fatigue | Паглынанне запасу сіл | custom |
| What happened? | Што здарылася? | skyrim |
| Warrior | Ваяр | skyrim |
| Vampire | Вампір | skyrim |
| Spriggan | Спрыган | skyrim |
| Silence | Цішыня | skyrim |
| Refugee | Уцякач | skyrim |
| Morag Tong Boots | Боты Мораг Тонг | skyrim |
| Madness Bow | Лук Вар'яцтва | skyrim |
| I'm ready. | Я напагатове. | skyrim |
| Greater Soul Gem | Велізарны камень душ | skyrim |
| Go on. | Кажы. | skyrim |
| GateKeeper | Брамніца | skyrim |
| Fly Amanita | Мухамор | skyrim |
| Bone | Костка | custom |
| Blackwood Company Guard | Ахоўнік кампаніі "Чорны лес" | custom |
| Black Soul Gem | Чорны камень душ | skyrim |
| Absorb Health | аглынанне здароўя | custom |
| Yes, I have. | Так, валодаю. | skyrim |
| Wooden door | Драўляныя дзверы | skyrim |
| Why me? | Чаму я? | skyrim |
| What happens now? | Што адбудзецца цяпер? | skyrim |
| What do you mean? | Што ты маеш на ўвазе? | skyrim |
| What can I do? | Што я магу зрабіць? | skyrim |
| Weakness to Shock | Уразлівасць да электрычнасці | skyrim |
| Weakness to Poison | Уразлівасць да ядаў | skyrim |
| Weakness to Frost | Уразлівасць да мароза | skyrim |
| Thief | Злодзей | skyrim |
| Telekinesis | Тэлекінэз | skyrim |
| Storm Atronach | Навальнічны атранах | skyrim |
| Spell Absorption | Паглынанне чараў | skyrim |
| Sheogorath | Шэагорат | skyrim |
| None of your business. | То не твая справа. | skyrim |
| No, not right now. | Не, не зараз | skyrim |
| No, I don't think so. | Не, я гэтак не думаю. | skyrim |
| Nirnroot | Карэнь Нірна | skyrim |
| Mead | Мёд | skyrim |
| It's a deal. | Дамовіліся. | skyrim |
| Invisibility | Нябачнасць | skyrim |
| I'll think about it. | Я паразважаю над гэтым. | skyrim |
| Fortify Health | Павышэнне здароўя | skyrim |
| Flame Stalk | Вогненнае сцябло | skyrim |
| Entrance | Уваход | skyrim |
| Dunbarrow Cove | Данбараўская бухта | custom |
| Dread Zombie | Жахлівы Зомбі | skyrim |
| Cure Poison | Проціяддзе | skyrim |
| Courier | Ганец | skyrim |
| Common Soul Gem | Звычайны камень душ | skyrim |
| Chorrol | Корал | custom |
| Bound Sword | Часовы меч | skyrim |
| Bound Bow | Часовы лук | skyrim |
| Boots | Боты | skyrim |
| Apprentice | Вучань | skyrim |
| Altar | Алтар | custom |
| Absorb Magicka | Паглынанне магіі | custom |
| Wraith | Здань | skyrim |
| Why? | Чаму? | skyrim |
| What happened here? | Што тут здарылася? | skyrim |
| What do we do now? | Што мы робім далей? | skyrim |
| What are you talking about? | Што ты маеш на ўвазе? | skyrim |
| What are you doing here? | Што ты тут робіш? | skyrim |
| Wabbajack | Вабаджак | skyrim |
| Venison | Аленіна | skyrim |
| Vampire Scout | Вампір-выведніка | skyrim |
| Vampire Mage | Вампір-маг | skyrim |
| Vampire Dust | Прах вампіра | skyrim |
| Vampire Assassin | Вампір-забойца | skyrim |
| Turn Undead | Выгнанне Нежыці | skyrim |
| Troll Abilities | Troll abilities | skyrim |
| Torch | Паходня | skyrim |
| Thorn Hook | Учэпістая калючка | skyrim |
| Test | test | skyrim |
| Summon Ghost | Выклік Здані | skyrim |
| Summon Dremora | Выклік Дрэмора | skyrim |
| Steel Helmet | Сталёвы шалом | skyrim |
| Soul Trap | Пастка Душ | skyrim |
| Skooma | Скума | skyrim |
| Shock | Электрычнасць | skyrim |
| Script Effect | Script Effect | skyrim |
| Screaming Maw | Крыклівая ляпа | skyrim |
| Rot Scale | Гнілая лускавінка | skyrim |
| Resist Magic | Адпорнасць да чараў | skyrim |
| Pumpkin | Гарбуз | skyrim |
| Priest | Святар | skyrim |
| Pickpocket | Кішэнны крадзеж | skyrim |
| Not now. | Не зараз. | skyrim |
| Nightshade | Ліснік | skyrim |
| Mythic Dawn Bound Armor | Прызваныя даспехі Міфічнага Світанку | custom |
| Mysterium Xarxes | Містэрыюм Заркса | skyrim |
| Mehrunes Dagon | Мехрунэс Дагон | skyrim |
| Madness Shield | Шчыт Вар'яцтва | skyrim |
| Madness Helmet | Шалом Вар'яцтва | skyrim |
| Madness Gauntlets | Наручы Вар'яцтва | skyrim |
| Madness Boots | Боты Вар'яцтва | skyrim |
| Liminal Bridges | Пераходныя мосты | skyrim |
| Lightning | Маланка | skyrim |
| Let's go. | Хадзем. | skyrim |
| Lesser Soul Gem | Меншы камень душ | skyrim |
| Lead on. | Вядзі. | skyrim |
| I'll take it. | Я вазьму гэта. | skyrim |
| I don't think so. | Я так не думаю. | skyrim |
| Go on... | Кажы... | skyrim |
| Gate Control | Кіраванне брамай | custom |
| Garlic | Часнык | skyrim |
| Frenzy | Шалёнства | skyrim |
| Fork | Відэлец | skyrim |
| Elven Helmet | Эльфскі шалом | skyrim |
| Elder Scroll | Старажытны Скрутак | skyrim |
| Dragon Breath | Dragon breath | skyrim |
| Damage Health | Урон здароўю | skyrim |
| Cure Disease | Ацаленне ад хваробы | skyrim |
| Citizen | Грамадзянін | skyrim |
| Certainly. | Канешне. | skyrim |
| Brown Bear | Карычневы мядзьведзь | skyrim |
| Broom | Мятла | skyrim |
| Bound Axe | Часовая сякера | skyrim |
| Boar | Вепрук | skyrim |
| Blades Shield | Шчыт Клінкоў | skyrim |
| Blades Helmet | Шалом Клінкоў | skyrim |
| Atronach Frost | Мароз атранаха | custom |
| Arch-Mage | Архімаг | skyrim |
| Anvil | Кавадла | skyrim |
| All right. | Добра. | skyrim |
| Aleswell | Эльсвел | custom |
| urgent task | Тэрміновае заданне | custom |
| added. | - дабаўлена. | custom |
| You cannot wait when enemies are nearby. | Вы не можаце чакаць, калі побач знаходзяцца ворагі. | custom |
| You cannot sleep with enemies nearby. | Вы не можаце спаць, калі побач ворагі. | custom |
| Yield | Здацца | skyrim |
| Yes | Так | skyrim |
| Wolf | Воўк | skyrim |
| Wizard | Чарадзей | skyrim |
| Wine | Віно | skyrim |
| Why do you care? | А табе што да таго? | skyrim |
| What now? | Што цяпер? | skyrim |
| What is this place? | Што гэта за месца? | skyrim |
| What do you want with me? | Што табе патрэбна ад мяне? | skyrim |
| What do you want me to do? | Што мне трэба зрабіць? | skyrim |
| Watchman | Брамнік | skyrim |
| Volendrung | Волендранг | skyrim |
| Void Salts | Пустотныя солі | skyrim |
| Tsunami Gate Control | Кіраванне брамай цунамі | custom |
| Troll Fat | Тлушч троля | skyrim |
| Tripwire | Расцяжка | skyrim |
| Trials of St. Alessia | Выпрабаванні святой Алесіі | skyrim |
| Training | Практыкаванне | skyrim |
| Tornado Gate Control | Кіраванне брамай тарнада | custom |
| Tongs | Абцугі | skyrim |
| Tomato | Памідор | skyrim |
| Thieves Guild | Гільдыя Зладзеяў | skyrim |
| The Madness of Pelagius | Вар'яцтва Пелагіюса | skyrim |
| Taproot | Стрыжнявы карэнь | skyrim |
| Steel Warhammer | Сталёвы молат | skyrim |
| Steel Shield | Сталёвы шчыт | skyrim |
| Steel Arrow | Сталёвая страла | skyrim |
| Staada | Стаада | skyrim |
| Soul Tomato | Памідор душ | skyrim |
| Sorcerer | Чарадзей | skyrim |
| Slaughterfish | Рыба-забойца | skyrim |
| Skeleton Key | Шкілетны Ключ | skyrim |
| Sithis | Сіціс | skyrim |
| Silver Goblet | Срэбны келіх | skyrim |
| Silver Bowl | Міса | skyrim |
| Shrine of Nocturnal | Свяцілішча Накцюрнал | skyrim |
| Shrine of Mephala | Свяцілішча Мефалы | skyrim |
| Shrine of Azura | Свяцілішча Азуры | skyrim |
| Scroll | Скрутак | skyrim |
| Scout | Выведнік | skyrim |
| Scar-Tail | Хвост са Шнарам | custom |
| Sanguine Rose | Ружа Сангвіна | skyrim |
| Sancre Tor, Catacombs | Санкр Тор, Катакомбы | custom |
| Ring of Disrobing | Пярсцёнак агольвання | skyrim |
| Resist magic | Адпорнасць да чараў | skyrim |
| Resist Poison | Трываласць да ядаў | skyrim |
| Resist Frost | Супраціўленне марозу | custom |
| Reanimate | Падняцце | skyrim |
| Rage | Раз'юшанасць | skyrim |
| Quill | Пяро | skyrim |
| Press Block | Націснуць блок | custom |
| Potato | Бульбіна | skyrim |
| Pilgrimage | Паломніцтва | skyrim |
| Pickaxe | Кірка | skyrim |
| Petty Soul Gem | Дробны камень душ | skyrim |
| Orcish Shield | Оркскі шчыт | skyrim |
| Orcish Helmet | Оркскі шалом | skyrim |
| Orc | Орк | skyrim |
| Novice | Навічок | skyrim |
| Nothing. | Нічога. | skyrim |
| Not really. | Не зусім. | skyrim |
| Not a chance. | І гаворкі быць не можа. | skyrim |
| No thanks. | Не, дзякуй. | skyrim |
| Nightblade | Клінок Ночы | skyrim |
| Mysterious Note | Таямнічая цыдулка | skyrim |
| Miner | Шахтар | skyrim |
| Maybe later. | Мабыць, пазней. | skyrim |
| Master-Wizard | Master-Wizard | skyrim |
| Master | Майстар | skyrim |
| Madness Ore | Руда Вар'яцтва | skyrim |
| Madness Arrow | Страла Вар'яцтва | skyrim |
| Lightning Storm | Навальніца | skyrim |
| Lightning Bolt | Маланка | skyrim |
| Lever | Вагар | skyrim |
| Let me think about it. | Дай мне падумаць аб гэтым. | skyrim |
| Leek | Цыбуля | skyrim |
| Leather Helmet | Скураны шалом | skyrim |
| Landslide Gate Control | Кіраванне абвалам | custom |
| Khajiit | Каджыт | skyrim |
| Iron Warhammer | Жалезны молат | skyrim |
| Iron War Axe | Жалезная сякера | skyrim |
| Iron Shield | Жалезны шчыт | skyrim |
| Iron Helmet | Жалезны шалом | skyrim |
| Inkwell | Каламар | skyrim |
| If you say so. | Як скажаш. | skyrim |
| Ice Storm | Ільдзяны Шторм | skyrim |
| I'm ready. Let's go. | Можна пачынаць. | skyrim |
| I'm ready when you are. | Я гатовая, калі і ты напагатове. | skyrim |
| I'm listening. | Я слухаю. | skyrim |
| I'll do it. | Я зраблю гэта. | skyrim |
| Human Heart | Чалавечае сэрца | skyrim |
| How can I help? | Як я магу дапамагчы? | skyrim |
| Hollowed-Out Rock | Парожні камень | skyrim |
| Hero | Герой | skyrim |
| Here you are. | Трымай. | skyrim |
| Have a coin, beggar. | Трымай манетку. | custom |
| Glow Dust | Святлівы пыл | skyrim |
| Glass Warhammer | Шкляны молат | skyrim |
| Glass Shield | Шкляны шчыт | skyrim |
| Glass Helmet | Шкляны шалом | skyrim |
| Glass Bow | Шкляны лук | skyrim |
| Fur Helmet | Футравы шалом | skyrim |
| Frost Salts | Марозныя солі | skyrim |
| Frost Atronach | Марозны атранах | skyrim |
| Flame Atronach | Вогненны атранах | skyrim |
| Fireball | Вогненны Шар | skyrim |
| Fire Storm | Вогненны Шторм | skyrim |
| Fire Ball | Вогненны Шар | skyrim |
| Exit | Выхад | custom |
| Evoker | Evoker | skyrim |
| Eruption Gate Control | Кіраванне брамай вывяржэння | custom |
| Elven Shield | Эльфскі шчыт | skyrim |
| Elven Gauntlets | Эльфскія пальчаткі | skyrim |
| Elven Bow | Эльфскі лук | skyrim |
| Elven Boots | Эльфскія боты | skyrim |
| Ectoplasm | Эктаплазма | skyrim |
| Ebony War Axe | Эбанітавая сякера | skyrim |
| Ebony Shield | Эбанітавы шчыт | skyrim |
| Ebony Mace | Эбанітавая булава | skyrim |
| Ebony Helmet | Эбанітавы шалом | skyrim |
| Ebony Bow | Эбанітавы лук | skyrim |
| Dremora | Дрэмора | skyrim |
| Dining Hall | Абедзенная зала | custom |
| Dark Brotherhood | Цёмны Хаўрус | skyrim |
| Daedric Shield | Шчыт дэйдра | skyrim |
| Daedric Helmet | Шалом дэйдра | skyrim |
| Daedric Gauntlets | Пальчаткі дэйдра | skyrim |
| Daedric Bow | Лук дэйдра | skyrim |
| Daedra Heart | Сэрца дэйдра | skyrim |
| Claw Gate | Брама кіпцюра | custom |
| Clairvoyance | Праніклівасць | skyrim |
| Charm | Абаянне | skyrim |
| Carrot | Морква | skyrim |
| Captain's Quarters | Апартаменты капітана | custom |
| Candlelight | Святло свечкі | skyrim |
| Bones | Косці | custom |
| Blizzard | Буран | skyrim |
| Blessing of Talos | Дабраславенне Таласа | skyrim |
| Blades Gauntlets | Пальчаткі Клінкоў | skyrim |
| Blades Boots | Боты Клінкоў | skyrim |
| Azura | Азура | skyrim |
| Atronach Storm | Шторм атранаха | custom |
| Atrabhi | Атрабі | custom |
| Argonian Bloodwine | Арганіянскае Крывавае віно | skyrim |
| Argonian | Арганіянец | skyrim |
| Arena Combatants Ability | Здольнасць байцоў Арэны | custom |
| Anvil Castle | Замак Анвіла | custom |
| Amusei | Амусей | custom |
| Amelion Tomb | Склеп Амеліёнаў | custom |
| Amber Sword | Бурштынавы меч | skyrim |
| Amber Shield | Бурштынавы шчыт | skyrim |
| Amber Mace | Бурштынавая булава | skyrim |
| Amber Helmet | Бурштынавы шалом | skyrim |
| Amber Gauntlets | Бурштынавыя наручы | skyrim |
| Amber Bow | Бурштынавы лук | skyrim |
| Amber Boots | Бурштынавыя боты | skyrim |
| Amber Arrow | Бурштынавая страла | skyrim |
| Amber | Бурштын | skyrim |
| Amantius Allectus | Амантыус Алектус | custom |
| Aloe Vera Leaves | Лісце алоэ | custom |
| Alkanet Flower | Кветка алканета | custom |
| Ale | Эль | skyrim |
| Ajum-Kajin | Аджум-Каджын | custom |
| Ahdarji | Адарджы | custom |
| Agent | Agent | skyrim |
| Aerin's Camp | Лагер Эйрын | custom |
| Advancement | Павышэнне | custom |
| Adrian Decanius' House | Дом Адрыяна Дэканія | custom |
| Adept | Адэпт | skyrim |
| Absorb spells | Убіранне заклёнаў | skyrim |
| Abandoned House | Пакінуты дом | skyrim |
