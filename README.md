print("请输入打于2的正整数：")
s=int(input())
begin=1
end=2
middle=(s+1)/2
ssum=begin+end
output=[]
while begin<middle:
    if ssum==s:
        output.append([begin,end])
        end+=1
        ssum+=end
    elif ssum<s:
        end+=1
        ssum+=end
    else:
        ssum-=begin
        begin+=1
if len(output)!=0:
    print("有{0}个序列".format(len(output)))
    for i in range(0,len(output),1):
        print("序列{0}: ".format(i+1))
        for j in range(output[i][0],output[i][1]+1):
            print(j,end=',')
        print("\n")
else:
    print("没有满足条件的序列！！！！！！")print("Hello World!")#输出

