test_str="hello world"
readonly ro_str="test"
test_one(){
        echo "test_str in test_one is $test_str"
        test_str="happy"
        test_name="anony"
        unset test_set    # 撤销变量test_set，之后引用该变量就会为空
        echo "test_set in test_one is $test_set"
        ro_str="tset"     # 该变量被readonly修饰，不能修改其变量值，将会出现语法错误，直接退出函数，不执行下列命令
        echo "ro_str# yasuo0.2
