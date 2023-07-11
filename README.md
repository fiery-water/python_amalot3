# python_amalot3

def fibonachi(n):
    "Foydalanuvchidan son qabul qilib shu son miqdoriga teng keluvchi fibonachi sonni topuvchi funcsiya"
    fib_sonlar=[]
    for x in range(n):
        if x==0 or x==1:
            fib_sonlar.append(1)
        else:
            fib_sonlar.append(fib_sonlar[x-1]+fib_sonlar[x-2])
    return fib_sonlar
fib=fibonachi(int(input("n=")))
print("fibonachi sonlar ",fib)

def katta_harf(ismlar):
    natija=[]
    for ism in ismlar:
        natija.append(ism.title())
    return natija
ismlar=['mavlon','javlon','ibrohim']
ruyxat=katta_harf(ismlar)
print(ruyxat,ismlar)

def bahola(ismlar):
    baholar={}
    for ism in ismlar:
        baho=int(input(f"Talaba {ism.title()}ning bahosini kiriting: "))
        baholar[ism]=baho
    return baholar
ismlar=['mavlon','muslim',"og'abek",'firdavs']
talabalar=bahola(ismlar)
print(talabalar)
