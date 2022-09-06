def no_record_breaking_days(no_of_days,visitors):
    record_breaking_count=0
    previous_record=0
    for i in range(no_of_days):
        greaterthanpreviousday=i==0 or visitors[i]>previous_record
        greaterthanfollowingday=i==no_of_days-1 or visitors[i]>visitors[i+1]
        
        if (greaterthanpreviousday and greaterthanfollowingday):
            record_breaking_count+=1
    
        previous_record=max(previous_record,visitors[i])
    return record_breaking_count

t=int(input())
for i in range(1,t+1):
    no_of_days=int(input())
    visitors=list(map(int,input().split()))
    ans=no_record_breaking_days(no_of_days,visitors)
    print('Case#{}: {}'.format(i,ans))
