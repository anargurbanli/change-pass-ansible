# İstifadəçi şifrələrinin avtomatlaşdırılmış dəyişdirilməsi
Bu repozitori, istifadəçi şifrələrinin avtomatlaşdırılmış yenilənməsi üçün istifadə olunur. Repozitori virtual, fiziki və ya bulud texnologiyalarında yerləşən linux distributivli serverlər üzərinə istifadə edilə bilər. Tapşırıqlar, idarə edilən serverlərdə root səlahiyyətləri ilə icra edilməlidir. Playbook işə salınmazdan öncə redaktə edilərək "hosts" bölməsinə uyğun host adları qeyd edilməlidir.

İnstruksiya:

1. Playbook işə salınarkən şifrəsinin dəyişilməsi nəzərdə tutulan istifadəçi adı tələbi ilk sorğu olaraq çıxır və istifadəçi adı qeyd edilməlidir.

2. Növbəti sorğu, adı qeyd olunmuş istifadəçi üçün şifrə təyin etmək tələbidir.

3. Tələblər qeyd edildikdən sonra playbook işə düşür və sorğu zamanı adı qeyd olunan istifadəçini idarə olunan hostlarda axtarır, Əgər həmin istifadəçi mövcuddursa, yalnız o zaman qeyd olunan şifrəni istifadəçiyə təyin edir. Əks halda, əgər sistemdə elə bir istifadəçi yoxdursa, playbook heç bir əməliyyat icra etmir.