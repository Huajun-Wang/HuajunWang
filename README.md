This code corresponds to the paper Huajun Wang, Wenqian Li ,  "Fast ramp fraction loss SVM classifier with low computational complexity
 for pattern classification, 
Neural Networks, 2024"

If you are using our code, please give proper citation to the above given paper.

If there is any issue/bug in the code please write to huajunwang2023@163.com or optimization li@163.com.

The codes of the simulate data and real data are described as follows:

The code of synthetic data is named as "demonSythData.m".  
Running the "demonSythData.m" file can obtain the results of  synthetic data of our algorithm.

The code of real data is named as "demonRealData.m".  
Running the "demonRealData.m" file can obtain the results of  real data of our algorithm.

The input and output parameters of our algorithm are described as follows
 Input parameters:
       X    -- the sample data, dimension, \in\R^{m-by-n}; (required)
       y    -- the classes of the sample data, \in\R^m; (required)
               y_i \in {+1,-1}, i=1,2,...,m
       pars -- parameters (optional)

 pars:    Parameters are all OPTIONAL
             pars.eta   --  Starting point of eta \in\R^m,  (default, zeros(m,1))
             pars.alpha  --  A positive scalar in (2^-4,2^-6,...,2^4).(default, 1)
             pars.theta      --  A positive scalar in (sqrt(2)^-4,...,sqrt(2)^4).(default, 1)
             pars.maxit   --  Maximum number of iterations, (default,1000)
             pars.tol     --  Tolerance of the halting condition, (default,1e-3)

   Output parameters:
    Out.iter:        Number of iterations
    Out.time:        CPU time
    Out.wb:          The solution of the primal problem, namely the classifier
    Out.q:           The solution q
    Out.eta:         The solution eta
    Out.alpha:       The solution alpha
    Out.nsv:         Number of support vectors
    Out.s:           Sparsity level of the solution Out.alpha
    Out.acc:         Classification accuracy
    Out.error:       Classification error

The all real dataset can be downloaded as follows：the libsvm library：(https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/datasets/),
 the kaggle library：  (https://www.kaggle.com/datasets)   and  the uci library ：(http://archive.ics.uci.edu/ml/datasets.php)
