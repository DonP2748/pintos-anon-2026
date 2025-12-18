
___PROJECT 1: THREADS


### 1
pintos -v -k -T 60 --qemu  -- -q  run alarm-single

### 2
pintos -v -k -T 60 --qemu  -- -q  run alarm-multiple 

### 3
pintos -v -k -T 60 --qemu  -- -q  run alarm-simultaneous 

### 4
pintos -v -k -T 60 --qemu  -- -q  run alarm-priority 

### 5
pintos -v -k -T 60 --qemu  -- -q  run alarm-zero 

### 6
pintos -v -k -T 60 --qemu  -- -q  run alarm-negative 

### 7   
pintos -v -k -T 60 --qemu  -- -q  run priority-change 

### 8
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-one 

### 9
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-multiple 
### 10
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-multiple2

### 11
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-nest 
### 12
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-sema 

### 13
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-lower 

### 14
pintos -v -k -T 60 --qemu  -- -q  run priority-fifo 

### 15
pintos -v -k -T 60 --qemu  -- -q  run priority-preempt 

### 16
pintos -v -k -T 60 --qemu  -- -q  run priority-sema 

### 17
pintos -v -k -T 60 --qemu  -- -q  run priority-condvar 

### 18
pintos -v -k -T 60 --qemu  -- -q  run priority-donate-chain 

### 19
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-load-1 

### 20
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-load-60 

### 21
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-load-avg

### 22
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-recent-1 

### 23
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-fair-2 

### 24
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-fair-20 

### 25
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-nice-2 

### 26
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-nice-10 

### 27
pintos -v -k -T 480 --qemu  -- -q -mlfqs run mlfqs-block 

___PROJECT 2: USERPROG



pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-none -a args-none -- -q  -f run args-none  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-single -a args-single -- -q  -f run 'args-single onearg'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-multiple -a args-multiple -- -q  -f run 'args-multiple some arguments for you!'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-many -a args-many -- -q  -f run 'args-many a b c d e f g h i j k l m n o p q r s t u v'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-dbl-space -a args-dbl-space -- -q  -f run 'args-dbl-space two  spaces!'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-bad-sp -a sc-bad-sp -- -q  -f run sc-bad-sp  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-bad-arg -a sc-bad-arg -- -q  -f run sc-bad-arg  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary -a sc-boundary -- -q  -f run sc-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary-2 -a sc-boundary-2 -- -q  -f run sc-boundary-2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary-3 -a sc-boundary-3 -- -q  -f run sc-boundary-3  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/halt -a halt -- -q  -f run halt  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exit -a exit -- -q  -f run exit  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-normal -a create-normal -- -q  -f run create-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-empty -a create-empty -- -q  -f run create-empty  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-null -a create-null -- -q  -f run create-null  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-bad-ptr -a create-bad-ptr -- -q  -f run create-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-long -a create-long -- -q  -f run create-long  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-exists -a create-exists -- -q  -f run create-exists  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-bound -a create-bound -- -q  -f run create-bound  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-normal -a open-normal -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run open-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-missing -a open-missing -- -q  -f run open-missing  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-boundary -a open-boundary -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run open-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-empty -a open-empty -- -q  -f run open-empty  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-null -a open-null -- -q  -f run open-null  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-bad-ptr -a open-bad-ptr -- -q  -f run open-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-twice -a open-twice -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run open-twice  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-normal -a close-normal -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run close-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-twice -a close-twice -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run close-twice  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-stdin -a close-stdin -- -q  -f run close-stdin  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-stdout -a close-stdout -- -q  -f run close-stdout  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-bad-fd -a close-bad-fd -- -q  -f run close-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-normal -a read-normal -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run read-normal 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-bad-ptr -a read-bad-ptr -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run read-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-boundary -a read-boundary -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run read-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-zero -a read-zero -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run read-zero  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-stdout -a read-stdout -- -q  -f run read-stdout  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-bad-fd -a read-bad-fd -- -q  -f run read-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-normal -a write-normal -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run write-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-bad-ptr -a write-bad-ptr -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run write-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-boundary -a write-boundary -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run write-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-zero -a write-zero -p ../../tests/userprog/sample.txt -a sample.txt -- -q  -f run write-zero  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-stdin -a write-stdin -- -q  -f run write-stdin  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-bad-fd -a write-bad-fd -- -q  -f run write-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-once -a exec-once -p tests/userprog/child-simple -a child-simple -- -q  -f run exec-once  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-arg -a exec-arg -p tests/userprog/child-args -a child-args -- -q  -f run exec-arg  
pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound -a exec-bound -p tests/userprog/child-args -a child-args -- -q  -f run exec-bound  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound-2 -a exec-bound-2 -- -q  -f run exec-bound-2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound-3 -a exec-bound-3 -- -q  -f run exec-bound-3  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-multiple -a exec-multiple -p tests/userprog/child-simple -a child-simple -- -q  -f run exec-multiple  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-missing -a exec-missing -- -q  -f run exec-missing  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bad-ptr -a exec-bad-ptr -- -q  -f run exec-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-simple -a wait-simple -p tests/userprog/child-simple -a child-simple -- -q  -f run wait-simple  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-twice -a wait-twice -p tests/userprog/child-simple -a child-simple -- -q  -f run wait-twice  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-killed -a wait-killed -p tests/userprog/child-bad -a child-bad -- -q  -f run wait-killed  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-bad-pid -a wait-bad-pid -- -q  -f run wait-bad-pid  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/multi-recurse -a multi-recurse -- -q  -f run 'multi-recurse 15'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/multi-child-fd -a multi-child-fd -p ../../tests/userprog/sample.txt -a sample.txt -p tests/userprog/child-close -a child-close -- -q  -f run multi-child-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-simple -a rox-simple -- -q  -f run rox-simple  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-child -a rox-child -p tests/userprog/child-rox -a child-rox -- -q  -f run rox-child  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-multichild -a rox-multichild -p tests/userprog/child-rox -a child-rox -- -q  -f run rox-multichild  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-read -a bad-read -- -q  -f run bad-read  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-write -a bad-write -- -q  -f run bad-write  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-read2 -a bad-read2 -- -q  -f run bad-read2  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-write2 -a bad-write2 -- -q  -f run bad-write2  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-jump -a bad-jump -- -q  -f run bad-jump  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-jump2 -a bad-jump2 -- -q  -f run bad-jump2  

pintos -v -k -T 360 --qemu  --filesys-size=2 -p tests/userprog/no-vm/multi-oom -a multi-oom -- -q  -f run multi-oom  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-create -a lg-create -- -q  -f run lg-create  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-full -a lg-full -- -q  -f run lg-full  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-random -a lg-random -- -q  -f run lg-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-seq-block -a lg-seq-block -- -q  -f run lg-seq-block  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-seq-random -a lg-seq-random -- -q  -f run lg-seq-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-create -a sm-create -- -q  -f run sm-create  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-full -a sm-full -- -q  -f run sm-full  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-random -a sm-random -- -q  -f run sm-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-seq-block -a sm-seq-block -- -q  -f run sm-seq-block  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-seq-random -a sm-seq-random -- -q  -f run sm-seq-random  

pintos -v -k -T 300 --qemu  --filesys-size=2 -p tests/filesys/base/syn-read -a syn-read -p tests/filesys/base/child-syn-read -a child-syn-read -- -q  -f run syn-read  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/syn-remove -a syn-remove -- -q  -f run syn-remove  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/syn-write -a syn-write -p tests/filesys/base/child-syn-wrt -a child-syn-wrt -- -q  -f run syn-write  

___PROJECT 3: VM



pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-none -a args-none --swap-size=4 -- -q  -f run args-none  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-single -a args-single --swap-size=4 -- -q  -f run 'args-single onearg' 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-multiple -a args-multiple --swap-size=4 -- -q  -f run 'args-multiple some arguments for you!' < /dt

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-many -a args-many --swap-size=4 -- -q  -f run 'args-many a b c d e f g h i j k l m n o p q r s t u v w x y z'


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-dbl-space -a args-dbl-space --swap-size=4 -- -q  -f run 'args-dbl-space two  spaces!' 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-bad-sp -a sc-bad-sp --swap-size=4 -- -q  -f run sc-bad-sp 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-bad-arg -a sc-bad-arg --swap-size=4 -- -q  -f run sc-bad-arg 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary -a sc-boundary --swap-size=4 -- -q  -f run sc-boundary 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary-2 -a sc-boundary-2 --swap-size=4 -- -q  -f run sc-boundary-2 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary-3 -a sc-boundary-3 --swap-size=4 -- -q  -f run sc-boundary-3 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/halt -a halt --swap-size=4 -- -q  -f run halt 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exit -a exit --swap-size=4 -- -q  -f run exit 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-normal -a create-normal --swap-size=4 -- -q  -f run create-normal 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-empty -a create-empty --swap-size=4 -- -q  -f run create-empty 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-null -a create-null --swap-size=4 -- -q  -f run create-null 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-bad-ptr -a create-bad-ptr --swap-size=4 -- -q  -f run create-bad-ptr 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-long -a create-long --swap-size=4 -- -q  -f run create-long 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-exists -a create-exists --swap-size=4 -- -q  -f run create-exists 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-bound -a create-bound --swap-size=4 -- -q  -f run create-bound 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-normal -a open-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run open-normal


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-missing -a open-missing --swap-size=4 -- -q  -f run open-missing 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-boundary -a open-boundary -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run open-boundary 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-empty -a open-empty --swap-size=4 -- -q  -f run open-empty 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-null -a open-null --swap-size=4 -- -q  -f run open-null 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-bad-ptr -a open-bad-ptr --swap-size=4 -- -q  -f run open-bad-ptr 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-twice -a open-twice -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run open-twice


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-normal -a close-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run close-normal


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-twice -a close-twice -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run close-twice


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-stdin -a close-stdin --swap-size=4 -- -q  -f run close-stdin 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-stdout -a close-stdout --swap-size=4 -- -q  -f run close-stdout 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-bad-fd -a close-bad-fd --swap-size=4 -- -q  -f run close-bad-fd 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-normal -a read-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-normal


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-bad-ptr -a read-bad-ptr -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-bad-ptr


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-boundary -a read-boundary -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-boundary


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-zero -a read-zero -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-zero


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-stdout -a read-stdout --swap-size=4 -- -q  -f run read-stdout 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-bad-fd -a read-bad-fd --swap-size=4 -- -q  -f run read-bad-fd 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-normal -a write-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-normal


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-bad-ptr -a write-bad-ptr -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-bad-ptr


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-boundary -a write-boundary -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-boundary


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-zero -a write-zero -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-zero


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-stdin -a write-stdin --swap-size=4 -- -q  -f run write-stdin 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-bad-fd -a write-bad-fd --swap-size=4 -- -q  -f run write-bad-fd 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-once -a exec-once -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run  exec-once


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-arg -a exec-arg -p tests/userprog/child-args -a child-args --swap-size=4 -- -q  -f run exec-arg 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound -a exec-bound -p tests/userprog/child-args -a child-args --swap-size=4 -- -q  -f run exec-bound


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound-2 -a exec-bound-2 --swap-size=4 -- -q  -f run exec-bound-2


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound-3 -a exec-bound-3 --swap-size=4 -- -q  -f run exec-bound-3 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-multiple -a exec-multiple -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run exec-multiple


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-missing -a exec-missing --swap-size=4 -- -q  -f run exec-missing 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bad-ptr -a exec-bad-ptr --swap-size=4 -- -q  -f run exec-bad-ptr 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-simple -a wait-simple -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run wait-simple


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-twice -a wait-twice -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run wait-twice


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-killed -a wait-killed -p tests/userprog/child-bad -a child-bad --swap-size=4 -- -q  -f run wait-killed


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-bad-pid -a wait-bad-pid --swap-size=4 -- -q  -f run wait-bad-pid 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/multi-recurse -a multi-recurse --swap-size=4 -- -q  -f run 'multi-recurse 15'


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/multi-child-fd -a multi-child-fd -p ../../tests/userprog/sample.txt -a sample.txt -p tests/userprog/chi????


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-simple -a rox-simple --swap-size=4 -- -q  -f run rox-simple 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-child -a rox-child -p tests/userprog/child-rox -a child-rox --swap-size=4 -- -q  -f run rox-child 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-multichild -a rox-multichild -p tests/userprog/child-rox -a child-rox --swap-size=4 -- -q  -f run rox-multichild


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-read -a bad-read --swap-size=4 -- -q  -f run bad-read  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-write -a bad-write --swap-size=4 -- -q  -f run bad-write  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-read2 -a bad-read2 --swap-size=4 -- -q  -f run bad-read2  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-write2 -a bad-write2 --swap-size=4 -- -q  -f run bad-write2  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-jump -a bad-jump --swap-size=4 -- -q  -f run bad-jump  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-jump2 -a bad-jump2 --swap-size=4 -- -q  -f run bad-jump2  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-stack -a pt-grow-stack --swap-size=4 -- -q  -f run pt-grow-stack  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-pusha -a pt-grow-pusha --swap-size=4 -- -q  -f run pt-grow-pusha  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-bad -a pt-grow-bad --swap-size=4 -- -q  -f run pt-grow-bad  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-big-stk-obj -a pt-big-stk-obj --swap-size=4 -- -q  -f run pt-big-stk-obj  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-bad-addr -a pt-bad-addr --swap-size=4 -- -q  -f run pt-bad-addr  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-bad-read -a pt-bad-read -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run pt-bad-read


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-write-code -a pt-write-code --swap-size=4 -- -q  -f run pt-write-code  


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-write-code2 -a pt-write-code2 -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run pt-write-code2


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-stk-sc -a pt-grow-stk-sc --swap-size=4 -- -q  -f run pt-grow-stk-sc  

pintos -v -k -T 300 --qemu  --filesys-size=2 -p tests/vm/page-linear -a page-linear --swap-size=4 -- -q  -f run page-linear  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/page-parallel -a page-parallel -p tests/vm/child-linear -a child-linear --swap-size=4 -- -q  -f run page-parallel

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/page-merge-seq -a page-merge-seq -p tests/vm/child-sort -a child-sort --swap-size=4 -- -q  -f run page-merge-seq

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/page-merge-par -a page-merge-par -p tests/vm/child-sort -a child-sort --swap-size=4 -- -q  -f run page-merge-par

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/page-merge-stk -a page-merge-stk -p tests/vm/child-qsort -a child-qsort --swap-size=4 -- -q  -f run page-merge-stk 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/page-merge-mm -a page-merge-mm -p tests/vm/child-qsort-mm -a child-qsort-mm --swap-size=4 -- -q  -f run page-merge-mm

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/page-shuffle -a page-shuffle --swap-size=4 -- -q  -f run page-shuffle  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-read -a mmap-read -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-read 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-close -a mmap-close -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-close < t

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-unmap -a mmap-unmap -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-unmap 


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-overlap -a mmap-overlap -p tests/vm/zeros -a zeros --swap-size=4 -- -q  -f run mmap-overlap < /dev/null t


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-twice -a mmap-twice -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-twice < t

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-write -a mmap-write --swap-size=4 -- -q  -f run mmap-write 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-exit -a mmap-exit -p tests/vm/child-mm-wrt -a child-mm-wrt --swap-size=4 -- -q  -f run mmap-exit 

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/mmap-shuffle -a mmap-shuffle --swap-size=4 -- -q  -f run mmap-shuffle  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-bad-fd -a mmap-bad-fd --swap-size=4 -- -q  -f run mmap-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-clean -a mmap-clean -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-clean

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-inherit -a mmap-inherit -p ../../tests/vm/sample.txt -a sample.txt -p tests/vm/child-inherit -a child-int

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-misalign -a mmap-misalign -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-misalign

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-null -a mmap-null -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-null 

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-over-code -a mmap-over-code -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-t

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-over-data -a mmap-over-data -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-t

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-over-stk -a mmap-over-stk -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-ovt

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-remove -a mmap-remove -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-removet

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-zero -a mmap-zero --swap-size=4 -- -q  -f run mmap-zero  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-create -a lg-create --swap-size=4 -- -q  -f run lg-create  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-full -a lg-full --swap-size=4 -- -q  -f run lg-full  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-random -a lg-random --swap-size=4 -- -q  -f run lg-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-seq-block -a lg-seq-block --swap-size=4 -- -q  -f run lg-seq-block  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-seq-random -a lg-seq-random --swap-size=4 -- -q  -f run lg-seq-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-create -a sm-create --swap-size=4 -- -q  -f run sm-create  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-full -a sm-full --swap-size=4 -- -q  -f run sm-full  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-random -a sm-random --swap-size=4 -- -q  -f run sm-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-seq-block -a sm-seq-block --swap-size=4 -- -q  -f run sm-seq-block  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-seq-random -a sm-seq-random --swap-size=4 -- -q  -f run sm-seq-random  

pintos -v -k -T 300 --qemu  --filesys-size=2 -p tests/filesys/base/syn-read -a syn-read -p tests/filesys/base/child-syn-read -a child-syn-read --swap-size=4 -- -q  -f run syn-read

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/syn-remove -a syn-remove --swap-size=4 -- -q  -f run syn-remove  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/syn-write -a syn-write -p tests/filesys/base/child-syn-wrt -a child-syn-wrt --swap-size=4 -- -q  -f run syn-write

___PROJECT 4: FILESYS



pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-none -a args-none --swap-size=4 -- -q  -f run args-none  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-single -a args-single --swap-size=4 -- -q  -f run 'args-single onearg'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-multiple -a args-multiple --swap-size=4 -- -q  -f run 'args-multiple some arguments for you!'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-many -a args-many --swap-size=4 -- -q  -f run 'args-many a b c d e f g h i j k l m n o p q r s t u v'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/args-dbl-space -a args-dbl-space --swap-size=4 -- -q  -f run 'args-dbl-space two  spaces!'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-bad-sp -a sc-bad-sp --swap-size=4 -- -q  -f run sc-bad-sp  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-bad-arg -a sc-bad-arg --swap-size=4 -- -q  -f run sc-bad-arg  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary -a sc-boundary --swap-size=4 -- -q  -f run sc-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary-2 -a sc-boundary-2 --swap-size=4 -- -q  -f run sc-boundary-2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/sc-boundary-3 -a sc-boundary-3 --swap-size=4 -- -q  -f run sc-boundary-3  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/halt -a halt --swap-size=4 -- -q  -f run halt  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exit -a exit --swap-size=4 -- -q  -f run exit  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-normal -a create-normal --swap-size=4 -- -q  -f run create-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-empty -a create-empty --swap-size=4 -- -q  -f run create-empty  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-null -a create-null --swap-size=4 -- -q  -f run create-null  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-bad-ptr -a create-bad-ptr --swap-size=4 -- -q  -f run create-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-long -a create-long --swap-size=4 -- -q  -f run create-long  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-exists -a create-exists --swap-size=4 -- -q  -f run create-exists  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/create-bound -a create-bound --swap-size=4 -- -q  -f run create-bound  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-normal -a open-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run open-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-missing -a open-missing --swap-size=4 -- -q  -f run open-missing  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-boundary -a open-boundary -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run open-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-empty -a open-empty --swap-size=4 -- -q  -f run open-empty  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-null -a open-null --swap-size=4 -- -q  -f run open-null  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-bad-ptr -a open-bad-ptr --swap-size=4 -- -q  -f run open-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/open-twice -a open-twice -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run open-twice  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-normal -a close-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run close-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-twice -a close-twice -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run close-twice  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-stdin -a close-stdin --swap-size=4 -- -q  -f run close-stdin  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-stdout -a close-stdout --swap-size=4 -- -q  -f run close-stdout  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/close-bad-fd -a close-bad-fd --swap-size=4 -- -q  -f run close-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-normal -a read-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-bad-ptr -a read-bad-ptr -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-boundary -a read-boundary -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-zero -a read-zero -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run read-zero  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-stdout -a read-stdout --swap-size=4 -- -q  -f run read-stdout  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/read-bad-fd -a read-bad-fd --swap-size=4 -- -q  -f run read-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-normal -a write-normal -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-normal  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-bad-ptr -a write-bad-ptr -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-boundary -a write-boundary -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-boundary  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-zero -a write-zero -p ../../tests/userprog/sample.txt -a sample.txt --swap-size=4 -- -q  -f run write-zero  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-stdin -a write-stdin --swap-size=4 -- -q  -f run write-stdin  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/write-bad-fd -a write-bad-fd --swap-size=4 -- -q  -f run write-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-once -a exec-once -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run exec-once  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-arg -a exec-arg -p tests/userprog/child-args -a child-args --swap-size=4 -- -q  -f run exec-arg  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound -a exec-bound -p tests/userprog/child-args -a child-args --swap-size=4 -- -q  -f run exec-bound  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound-2 -a exec-bound-2 --swap-size=4 -- -q  -f run exec-bound-2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bound-3 -a exec-bound-3 --swap-size=4 -- -q  -f run exec-bound-3  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-multiple -a exec-multiple -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run exec-multiple  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-missing -a exec-missing --swap-size=4 -- -q  -f run exec-missing  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/exec-bad-ptr -a exec-bad-ptr --swap-size=4 -- -q  -f run exec-bad-ptr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-simple -a wait-simple -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run wait-simple  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-twice -a wait-twice -p tests/userprog/child-simple -a child-simple --swap-size=4 -- -q  -f run wait-twice  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-killed -a wait-killed -p tests/userprog/child-bad -a child-bad --swap-size=4 -- -q  -f run wait-killed  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/wait-bad-pid -a wait-bad-pid --swap-size=4 -- -q  -f run wait-bad-pid  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/multi-recurse -a multi-recurse --swap-size=4 -- -q  -f run 'multi-recurse 15'  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/multi-child-fd -a multi-child-fd -p ../../tests/userprog/sample.txt -a sample.txt -p tests/userprog/child-close -a child-close --swap-size=4 -- -q  -f run multi-child-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-simple -a rox-simple --swap-size=4 -- -q  -f run rox-simple  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-child -a rox-child -p tests/userprog/child-rox -a child-rox --swap-size=4 -- -q  -f run rox-child  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/rox-multichild -a rox-multichild -p tests/userprog/child-rox -a child-rox --swap-size=4 -- -q  -f run rox-multichild  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-read -a bad-read --swap-size=4 -- -q  -f run bad-read  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-write -a bad-write --swap-size=4 -- -q  -f run bad-write  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-read2 -a bad-read2 --swap-size=4 -- -q  -f run bad-read2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-write2 -a bad-write2 --swap-size=4 -- -q  -f run bad-write2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-jump -a bad-jump --swap-size=4 -- -q  -f run bad-jump  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/userprog/bad-jump2 -a bad-jump2 --swap-size=4 -- -q  -f run bad-jump2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-create -a lg-create --swap-size=4 -- -q  -f run lg-create  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-full -a lg-full --swap-size=4 -- -q  -f run lg-full  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-random -a lg-random --swap-size=4 -- -q  -f run lg-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-seq-block -a lg-seq-block --swap-size=4 -- -q  -f run lg-seq-block  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/lg-seq-random -a lg-seq-random --swap-size=4 -- -q  -f run lg-seq-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-create -a sm-create --swap-size=4 -- -q  -f run sm-create  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-full -a sm-full --swap-size=4 -- -q  -f run sm-full  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-random -a sm-random --swap-size=4 -- -q  -f run sm-random  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-seq-block -a sm-seq-block --swap-size=4 -- -q  -f run sm-seq-block  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/sm-seq-random -a sm-seq-random --swap-size=4 -- -q  -f run sm-seq-random  

pintos -v -k -T 300 --qemu  --filesys-size=2 -p tests/filesys/base/syn-read -a syn-read -p tests/filesys/base/child-syn-read -a child-syn-read --swap-size=4 -- -q  -f run syn-read  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/syn-remove -a syn-remove --swap-size=4 -- -q  -f run syn-remove  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/filesys/base/syn-write -a syn-write -p tests/filesys/base/child-syn-wrt -a child-syn-wrt --swap-size=4 -- -q  -f run syn-write  

rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-empty-name -a dir-empty-name -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-empty-name  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-empty-name.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-mk-tree -a dir-mk-tree -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-mk-tree  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-mk-tree.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-mkdir -a dir-mkdir -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-mkdir  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-mkdir.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-open -a dir-open -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-open  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-open.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-over-file -a dir-over-file -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-over-file  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-over-file.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-rm-cwd -a dir-rm-cwd -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-rm-cwd  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-rm-cwd.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-rm-parent -a dir-rm-parent -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-rm-parent  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-rm-parent.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk


rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-rm-root -a dir-rm-root -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-rm-root  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-rm-root.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk


rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-rm-tree -a dir-rm-tree -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-rm-tree  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-rm-tree.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-rmdir -a dir-rmdir -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-rmdir  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-rmdir.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-under-file -a dir-under-file -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-under-file  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-under-file.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 150 --qemu  --disk=tmp.dsk -p tests/filesys/extended/dir-vine -a dir-vine -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run dir-vine  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/dir-vine.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-create -a grow-create -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-create  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-create.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk


rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-dir-lg -a grow-dir-lg -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-dir-lg  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-dir-lg.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-file-size -a grow-file-size -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-file-size  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-file-size.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-root-lg -a grow-root-lg -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-root-lg  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-root-lg.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-root-sm -a grow-root-sm -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-root-sm  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-root-sm.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-seq-lg -a grow-seq-lg -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-seq-lg  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-seq-lg.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-seq-sm -a grow-seq-sm -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-seq-sm  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-seq-sm.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-sparse -a grow-sparse -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-sparse  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-sparse.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-tell -a grow-tell -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-tell  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-tell.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/grow-two-files -a grow-two-files -p tests/filesys/extended/tar -a tar --swap-size=4 -- -q  -f run grow-two-files  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/grow-two-files.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk



rm -f tmp.dsk
pintos-mkdisk tmp.dsk --filesys-size=2
pintos -v -k -T 60 --qemu  --disk=tmp.dsk -p tests/filesys/extended/syn-rw -a syn-rw -p tests/filesys/extended/tar -a tar -p tests/filesys/extended/child-syn-rw -a child-syn-rw --swap-size=4 -- -q  -f run syn-rw  pintos -v -k -T 60  --qemu --disk=tmp.dsk -g fs.tar -a tests/filesys/extended/syn-rw.tar --swap-size=4 -- -q  run 'tar fs.tar /'  rm -f tmp.dsk


pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-stack -a pt-grow-stack --swap-size=4 -- -q  -f run pt-grow-stack  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-pusha -a pt-grow-pusha --swap-size=4 -- -q  -f run pt-grow-pusha  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-bad -a pt-grow-bad --swap-size=4 -- -q  -f run pt-grow-bad  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-big-stk-obj -a pt-big-stk-obj --swap-size=4 -- -q  -f run pt-big-stk-obj  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-bad-addr -a pt-bad-addr --swap-size=4 -- -q  -f run pt-bad-addr  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-bad-read -a pt-bad-read -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run pt-bad-read  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-write-code -a pt-write-code --swap-size=4 -- -q  -f run pt-write-code  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-write-code2 -a pt-write-code2 -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run pt-write-code2  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/pt-grow-stk-sc -a pt-grow-stk-sc --swap-size=4 -- -q  -f run pt-grow-stk-sc  

pintos -v -k -T 300 --qemu  --filesys-size=2 -p tests/vm/page-linear -a page-linear --swap-size=4 -- -q  -f run page-linear  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/page-parallel -a page-parallel -p tests/vm/child-linear -a child-linear --swap-size=4 -- -q  -f run page-parallel  

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/page-merge-seq -a page-merge-seq -p tests/vm/child-sort -a child-sort --swap-size=4 -- -q  -f run page-merge-seq  

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/page-merge-par -a page-merge-par -p tests/vm/child-sort -a child-sort --swap-size=4 -- -q  -f run page-merge-par  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/page-merge-stk -a page-merge-stk -p tests/vm/child-qsort -a child-qsort --swap-size=4 -- -q  -f run page-merge-stk  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/page-merge-mm -a page-merge-mm -p tests/vm/child-qsort-mm -a child-qsort-mm --swap-size=4 -- -q  -f run page-merge-mm  

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/page-shuffle -a page-shuffle --swap-size=4 -- -q  -f run page-shuffle  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-read -a mmap-read -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-read  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-close -a mmap-close -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-close  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-unmap -a mmap-unmap -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-unmap  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-overlap -a mmap-overlap -p tests/vm/zeros -a zeros --swap-size=4 -- -q  -f run mmap-overlap  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-twice -a mmap-twice -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-twice  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-write -a mmap-write --swap-size=4 -- -q  -f run mmap-write  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-exit -a mmap-exit -p tests/vm/child-mm-wrt -a child-mm-wrt --swap-size=4 -- -q  -f run mmap-exit  

pintos -v -k -T 600 --qemu  --filesys-size=2 -p tests/vm/mmap-shuffle -a mmap-shuffle --swap-size=4 -- -q  -f run mmap-shuffle  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-bad-fd -a mmap-bad-fd --swap-size=4 -- -q  -f run mmap-bad-fd  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-clean -a mmap-clean -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-clean  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-inherit -a mmap-inherit -p ../../tests/vm/sample.txt -a sample.txt -p tests/vm/child-inherit -a child-inherit --swap-size=4 -- -q  -f run mmap-inherit  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-misalign -a mmap-misalign -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-misalign  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-null -a mmap-null -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-null  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-over-code -a mmap-over-code -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-over-code  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-over-data -a mmap-over-data -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-over-data  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-over-stk -a mmap-over-stk -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-over-stk  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-remove -a mmap-remove -p ../../tests/vm/sample.txt -a sample.txt --swap-size=4 -- -q  -f run mmap-remove  

pintos -v -k -T 60 --qemu  --filesys-size=2 -p tests/vm/mmap-zero -a mmap-zero --swap-size=4 -- -q  -f run mmap-zero  

