 int DivisibleByEight(string s){
        //code here
        int n=s.length();
        if(n<3){// if length of string is less than three then make the lenghth of string is 3
            while(n<3){
                s='0'+s;
                n++;
            }
        }
        
        //our length is greater than equal to 3
        int number=0;
        for(int i=n-3;i<=n-1;i++){// last ke three number liyee aur unpe loop chalaya
            number=number*10+(s[i]-'0'); //number ko 10 se multiply kiya aur string ko no. mai convert kiyaa
        }
        if(number%8==0){
            return 1;
        }
        else{
            return -1;
        }
    }
