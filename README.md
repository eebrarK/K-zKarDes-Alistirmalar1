#soru-1
def say(elemanlar):
    if len(elemanlar) == 0:
        return "Hata: Boş liste!"
    return len(elemanlar)

#soru-2
def karakter_sayisi(s, ignore_case=False):
    if ignore_case:
        s = s.lower()
    
    karakter_dict = {}

    for karakter in s:
        if karakter.isalnum():  
            if karakter in karakter_dict:
                karakter_dict[karakter] = karakter_dict[karakter] + 1
            else:
                karakter_dict[karakter] = 1
    
    return karakter_dict

#soru-3
def filtre_ve_kareye_cevir(sayilar, esik):
    kareler = []  
    for sayi in sayilar:  
        if sayi > esik:  
            kareler.append(sayi * sayi)  
    return kareler  
