k = int(input("Enter value of k"))
X=[]
B=[]
X = np.array([input() for i in range(k)])

B = np.array([sum(i)/k for i in X])
parent_matrix = np.array([[0 for i in range(k)] for j in range(k)])



#Let X be a RV with parents U1,.....,Uk with Linear Gaussian CPD

#D
def LinearGaussianCPD(k):
    coeff = []
    final_list = []
    for i in range(k):
        temp_list=parent_matrix[:,i]
        for i in range(k):
            final_list.append(sum(np.multiply(temp_list,parent_matrix[:,i]))/k)
    print(final_list)
    
    A = np.array(final_list)
    
    inv_A = np.linalg.inv(A)
    
    coeff = np.linalg.inv(A).dot(B)
    
    print(coeff)
    
LinearGaussianCPD(k) 
