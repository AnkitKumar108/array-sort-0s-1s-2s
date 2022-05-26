# array-sort-0s-1s-2s




int l=0;
int m=0;
int h=n-1;

while(m<=h){
    int x=nums[m];
    if(x==0){
        swap(nums[l],nums[m]);
        l++;
        m++;
    }
    else if(x==1){
        m++;
    }
    else{
        swap(nums[h],nums[m]);
        h--;
    }
    
}


//another approach 


while(m<=h)
{
    if(a[m]==0){
        swap(a[l],a[m]);
        l++;
        m++;
    }
    if(a[m]==1){
        m++;
    }
    if(a[m]==2){
        swap(a[m],a[h]);
        
        h--;
    }
    
}
