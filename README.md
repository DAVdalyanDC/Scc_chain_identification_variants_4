Արտադրական շղթայի իդենտիֆիկացիա

Խնդրի դրվածքը

Հայտնի է որ բարդ սարքավորումների արտադրությունը անցնում է շատ փուլերով։
Օրինակ էլեկտրական միկրոսխեմաները պատրաստելու համար գոյություն ունեն իրարից
բավականին տարբեր փուլեր՝
1) Տեխնիկական առաջադրանքի պատրաստում,
2) Էլեկտրական սխեմայի նախագծում,
3) Էլեկտրական սխեմայի ստուգում (տրամաբանական ստուգում),
4) Էլեկտրական սխեմայի թարգմանություն դեպի չիպի նախագիծ,
5) Չիպի նախագծի վերիֆիկացիա (պատրաստելու հնարավորություն ստուգում,
պարազիտիկ տարրերի հեռացում),
6) Չիպի նախագծի հիման վրա բուն չիպի արտադրություն,
7) Պատրաստի չիպերի թեստավորում, եւ խոտանների դեն նետում։
Իդեպ, այդ փուլերը միշտ չէ որ հստակ հաջորդականությամբ են կատարվում։ Նշված
օրինակում 3-րդ փուլից հետո հնարավոր է պարզվի որ էլեկտրական սխեման ունի իր մեջ
ինչ-որ թերություններ, ու պետք է ոչ թե առաջ անցնել դեպի չիպի նախագծի
պատրաստում (4-րդ փուլ), այլ հետ գնալ դեպի եւս մեկ անգամ էլեկտրական սխեմայի
նախագծում (2-րդ փուլ)։ Բայց եթե էլեկտրական սխեման թերություններ չունի, ու մենք
անցել ենք չիպի նախագծի պատրաստման (4-րդ փուլ), այլեւս հնարավոր չի որ
ապագայում պարզվի որ էլեկտրական սխեման (2-րդ փուլ) կամ տեխնիկական
առաջադրանքը (1-րդ փուլ) թերի էին։
Մենք ներգրավված ենք մի արտադրական պրոցեսի մեջ, որն ունի N փուլեր։ Ամեն փուլի
համար հայտնի է թե իրենից հետո դեպի որ փուլ հնարավոր է անցում կատարվի։ Եվ
մենք պետք է գրենք ծրագիր որը կպատասխանի 2 հարցերի.

• Արդյո՞ք այդ արտադրական փուլերի մեջ կան այնպիսի պահեր, երբ անցնելով ինչ-
որ նոր փուլի այլեւս ոչ մի պարագայում հնարավոր չի հետ-վերադարձ կատարել

դեպի նախորդ փուլեր։
• Արդյո՞ք ընդհանուր արտադրական շղթան իրենից ներակայացնում է գծային
պրոցես, թե այն ունի ճյուղավորումներ եւ / կամ միացման կետեր?
Մեր դիտարկված օրինակի համար հնարավոր անցումներն են՝
1->2, 2->1, 2->3, 3->2, 3->4, 4->5, 5->4, 5->6, 6->7
Իսկ պատասխանը պետք է լինի հետեւյալը՝
1, 2, 3 փուլերում կարող ենք տեղափոխվել մեկից մյուսը,
4, 5 փուլերում նույնպես կարող ենք տեղափոխվել մեկից մյուսը,

6-րդ փուլից կարող ենք գնալ միայն դեպի 7,
7-րդ փուլից ոչ մի տեղ չենք կարող գնալ։
Այսինքն անվերադառնալի փուլերն են՝ 1, 4, 6, 7:
Եվ այո, այս պրոցեսը գծային է, քանի որ այդ 1, 4, 6, 7 փուլերով արտադրությունը
անցնելու է ամեն դեպքում, ու հենց այդ հաջորդականությամբ։

Մուտքային եւ ելքային տվյալներ

Մուտքային տվյալները սկսվում են N թվից, ոիրց հետո N տողերում գրված են այդ N
փուլերի անվանումները։ Այնուհետեւ նշվում է M թիվը, որից հետո M տողերում թվարկվում
են փուլից փուլ բոլոր հնարավոր անցումները։ Այդ M տողերից ամեն մեկը ունի «Ai Bi»
ֆորմատը եւ ցույց է տալիս որ «Ai» փուլից կարող ենք անցում կատարել դեպի «Bi»
փուլը։
Ելքում ծրագիրը պետք է տպի հետեւյալը՝
• L թիվը - «անվերադարձ» փուլերի քանակը,
• Նշի այն L հատ փուլերի անվանումները, որտեղ մուտք գործելուց հետո այլեւս
հնարավոր չէ վերադառնալ որեւէ նախորդ փուլի,
• Հաջորդ L տողերից ամեն մեկում թվարկի այն բոլոր փուլերը որոնցից հնարավոր է
վերադառնալ այդ հերթական՝ i-րդ անվերադարձ փուլ,
• Պատասխանի «այո / ոչ» այն հարցին, արդյո՞ք ընդհանուր արտադրությունը
իրենից ներկայացնում է գծային պրոցես։ Եթե այն ներկայացնում է գծային պրոցես,
պետք է նաեւ մեկ տողով թվարկել այդ L հատ փուլերը ըստ այն
հաջորդականության, որով իրենք կատարվելու են։





Լուծման տարբերակ 4

(adj. list, Kosaraju, DFS, reverse, in_out_degree)

Արտադրության փուլերը պետք է համարակալվեն [0, N) թվերով, եւ պետք է պահել
երկկողմանի արտապատկերում այդ ինդեքստներից դեպի փուլերի անունները եւ
հակառակը։ Ներսում ծրագիրը բոլոր հաշվարկները պետք է անի ըստ այդ ինդեքսների,
իսկ փուլերի անվանումները օգտագործի միայն ներմուծման եւ արտածման ժամանակ։

Փուլերը եւ իրենց միջեւ անցումները պետք է պահել որպես ուղորդված գրաֆ, որն էլ
ներկայացված լինի «adjacency list» կառուցվածքով։
Ուժեղ-կապակցված կոմպոնենտների հայտնաբերումը պետք է կատարել Kosaraju-ի
ալգորիթմով, որն իր հերթին տոպոլոգիական սորտավորումը պետք է կատարի DFS
ալգորիթմով։ Kosaraju-ի ալգորիթմի երկրորդ փուլի համար օգտագործել եղած
«adjacency list»-ը, տեղում իրեն շրջելով (այլ ոչ թե պատճենահանելով դեպի նոր
կցության ցուցակ)։
Ստուգումը, արդյո՞ք ընդհանուր արտադրությունը ներկայացնում է իրենից գծային
պրոցես, կատարել կոնդենսացնելով մուտքային գրաֆը, ու հաշվարկելով գագաթների
ստացված խմբերի մեջ մտնող եւ դուրս եկող կողերի քանակները։
Լուծումը պետք է կազմված լինի հետեւյալ դասերից (classes).
• Փուլերի անվանումները դեպի [0, N) ինդեքսներ, եւ հակառակը արտապատկերելու
համար,
• Գրաֆի պահման համար,
• DFS ալգորիթմի աշխատանքի, եւ իր արդյունքների պահման համար,
• Գրաֆի կողերի շրջման համար,
• Կոսարաջույի ալգորիթմի աշխատանքի համար, որն էլ իր հերթին պետք է դիմի
DFS ալգորիթմը աշխատեցնող դասին եւ գրաֆը շրջող դասին,
• Ընդհանուր արտադրությունը գծային պրոցես լինելու ստուգման համար։
