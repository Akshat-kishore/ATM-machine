# ATM-machine
# cook your dish here
if __name__ == '__main__':
    for _ in range(int(input())):
        n, k = map(int, input().split())
        A = list(map(int, input().split()))[:n]
        
        c = 0
        t = ''
        for i in A:
            if (i<=k-c) and (c != k):
                c+=i
                t+='1'
            
            else:
                t+='0'
        
        print(t)
