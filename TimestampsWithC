#include<stdio.h>

typedef struct timestamp{
    int dd,mm,yyyy;
    int hr,min,secs;
}tstamp;

void display(tstamp t){
    printf("TIMESTAMP -> %d/%d/%d  %.2d:%.2d:%.2d\n",t.dd,t.mm,t.yyyy,t.hr,t.min,t.secs);
}

int timeCmp(tstamp t1, tstamp t2){
    if(t1.yyyy>t2.yyyy){           //Comparing years
        return 1;
    }
    if(t1.yyyy<t2.yyyy){
        return -1;
    }
    if(t1.mm>t2.mm){              //Comparing months
        return 1;
    }
    if(t1.mm<t2.mm){
        return -1;
    }
    if(t1.dd>t2.dd){              //Comparing days
        return 1;
    }
    if(t1.dd<t2.dd){
        return -1;
    }

    if(t1.hr>t2.hr){              //Comparing hours
        return 1;
    }
    if(t1.hr<t2.hr){
        return -1;
    }
    if(t1.min>t2.min){            //Comparing minutes
        return 1;
    }
    if(t1.min<t2.min){
        return -1;
    }
    if(t1.secs>t2.secs){          //Comparing seconds
        return 1;
    }
    if(t1.secs<t2.secs){
        return -1;
    }

    return 0;  //if timestamps are equal
}
 
int main(){
    tstamp t1 = {26,10,2022,14,22,45};
    tstamp t2 = {28,10,2022,10,00,00};
    display(t1);
    display(t2);

    int CmpResult = timeCmp(t1,t2);
    printf("Timestamp comparison function results: %d",CmpResult);
    return 0;
}
