

### **Solution**
The given differential equation is 

$$y''-y=6 \sin 2x$$

### **Step 1: Rewriting the Equation**

We can rewrite this equation in standard form. 

$$y''+y=6 \sin 2x$$

### **Step 2: Finding the Characteristic Equation**

The characteristic equation of the differential equation is given by 

$$r^2+1=0$$

This equation has two distinct real roots as 

$$r_1=-1, \quad r_2=1$$

### **Step 3: Finding the General Solution**

The general solution of the equation is given by 

$$y(x)=c_1e^{-x}+c_2e^x$$

### **Step 4: Finding the Particular Solution**

Using the method of variation of parameters, the particular solution of the equation is given by 

$$y_p(x)=\sin 2x \int \frac{6}{2}e^x \ dx - \cos 2x \int \frac{6}{2}e^{-x} \ dx$$

$$\implies y_p(x)=3e^x \sin 2x - 3e^{-x} \cos 2x$$

### **Step 5: Finding the Complete Solution**

The complete solution of the equation is given by 

$$y(x)=c_1e^{-x}+c_2e^x+3e^x \sin 2x - 3e^{-x} \cos 2x$$