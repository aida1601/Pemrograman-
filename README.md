def hitung_gaya(m,a):
    F = m*a
    return F

def hitung_massa(F,a):
    m = F/a
    return m

def hitung_percepatan(F,m):
    a = F/m
    return a

def main():
    print("program untuk menghitung Gaya")
    print("1. hitung gaya (F)")
    print("2. Hitung mmassa (m)")
    print("3. Hitung percepatan (a)")

    pilihan = input("masukkan pilihan 1/2/3/: ")

    if pilihan == "1":
        m = float(input("masukkan massa benda dalam kg :"))
        a = float(input("masukkan percepatan benda dalam m/s^2 :"))
        F = hitung_gaya(m,a)
        print(F"gaya benda sebesar: {F: .2f} N")

    elif pilihan == "2":
       F = float(input("masukkan gaya dalam N :"))
       a = float(input("masukkan percepatan dalam m/s^2 :"))  
       m = hitung_massa(F,a)
       print(F"massa benda sebesar: {m: .2f} kg")

    elif pilihan == "3":
        F = float(input("masukkan gaya dalam N :"))
        m = float(input("masukkan massa benda dalam kg :"))
        a = hitung_percepatan(F,m)
        print(F"percepatan benda sebesar: {a: .2f} m/s^2 :")

    else:
        print("pilihan tidak sesuai, silakan pilih 1/2/3")
if __name__ == "__main__":
    main()


    
