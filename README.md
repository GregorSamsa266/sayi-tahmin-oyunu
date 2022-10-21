# sayi-tahmin-oyunu
import random
sayı = random.randint(1,20)
can = 5
hak= 0

while can > 0:
    can -= 1
    hak += 1
    tahmin = int(input('Kullanıcı tahmini: '))
    if sayı == tahmin:
        print(f'Tebrikler {hak}. hakkınızda doğru cevap verdiniz.')
        break
    elif sayı > tahmin:
        print('Çık biraz çık.')
    else:
        print('Çok yükseklerdesin. Aşağı in bakalım.')
if can ==0:
    print(f'Canın bitti. Başka sefere artık.Doğru cevap: {sayı}')
