from re import split

tarih = input("lütfen gün ay yıl olarak bir tarih giriniz arada boşluk bırakarak: ")
def artıkYıl(yıl):
    if(yıl % 400 == 0) or (yıl % 4 == 0 and yıl % 100 != 0):
        return True
    return False

def yılınGünü(gün, ay, yıl):
    günler = [31,28,31,30,31,30,31,31,30,31,30,31]
    if artıkYıl(yıl):
        günler[1] = 29
    sıra = 0
    for i in range(ay - 1):
        sıra += günler[i]
    sıra += gün
    return  sıra

gün, ay, yıl = map( int, tarih.split()) # Girdiği veriyi gün, ay, yıl olarak ayır

print(yılınGünü(gün, ay, yıl))



