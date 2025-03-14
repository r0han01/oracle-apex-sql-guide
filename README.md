## **📌 Oracle APEX for SQL Practice & Development**  

###
![Screenshot from 2025-03-14 17-45-32](https://github.com/user-attachments/assets/3de01828-d295-4389-923b-97937edba308)
###

###

### **🚀 Why Use Oracle APEX Instead of Installing Locally?**  
Oracle APEX is a powerful, web-based **low-code platform** that eliminates the need to install **Oracle Database** on your local machine. Instead of dealing with complex installations, dependencies, and OS compatibility issues (like missing a `.deb` package for Ubuntu), you can directly use **Oracle APEX on Oracle Cloud** for free.  

✅ **No need to install EXE or DB setup**  
✅ **Works on Windows, macOS, Linux (Ubuntu, Fedora, etc.)**  
✅ **Instant access from a browser**  
✅ **Scalable & always up-to-date**  

---

## **🔧 How to Set Up Oracle APEX in Oracle Cloud**
Follow these steps to set up Oracle APEX for practicing SQL and building applications.

### **1️⃣ Sign Up for Oracle Cloud (Free)**
1. Go to [Oracle Cloud Sign-Up](https://www.oracle.com/cloud/free/)  
2. Create an account and verify your email.  
3. Sign in to the Oracle Cloud Console.  

### **2️⃣ Create an Autonomous Database**
1. Navigate to **Oracle Cloud Console** → **Autonomous Database**.  
2. Click **"Create Autonomous Database"**.  
3. Choose:  
   - **Database type:** APEX  
   - **Always Free:** ✅ (to avoid any cost)  
   - **Compute Auto Scaling:** Disabled (for now)  
4. Set a **secure password** for the database.  
5. Click **"Create"** and wait for provisioning.  

### **3️⃣ Launch APEX & Create Workspace**
1. In **Oracle Cloud Console**, go to **Developer Services → APEX Application Development**.  
2. Click **"Launch APEX"**.  
3. Click **"Create Workspace"** → Choose **New Schema**.  
4. Set **Workspace Name, Schema, and Password**.  
5. Sign in to your new workspace.  

🎉 **Done! You are now inside Oracle APEX and ready to practice SQL.**  

---

## **🐞 Troubleshooting & Common Errors**  

### **🚨 1. Database Connection Error (HTTP Status Code: 571)**
**Error Message:**  
```
The connection pool named: ORDS_PLSQL_GATEWAY encountered a network operation error: UCP-29: Failed to get a connection
```
✅ **Solution:**  
1. **Restart APEX Instance**:  
   - Oracle Cloud Console → **Developer Services → APEX Instances** → Click **Restart**.  
2. **Restart Autonomous Database**:  
   - Go to **Autonomous Database** → Click **Restart**.  
3. Wait a few minutes and try again.  

---

### **🚨 2. Workspace Login Issues**
**Issue:** Cannot log in to the workspace after creation.  
✅ **Solution:**  
- Ensure you are using the correct **Workspace Name** (not database name).  
- Try resetting the **ADMIN** password from the **Autonomous Database settings**.  

---

### **🚨 3. ORA-00942: Table or View Does Not Exist**
**Issue:** Running `SELECT * FROM table_name;` gives an error.  
✅ **Solution:**  
- Make sure the table exists:  
  ```sql
  SELECT table_name FROM user_tables;
  ```
- If not, create it first.  

---

## **📜 Basic SQL Commands for Practice**
Here are some basic SQL queries to get started with APEX.

### **🔹 1️⃣ Check Current Date**
```sql
SELECT SYSDATE FROM DUAL;
```

### **🔹 2️⃣ Create a Table**
```sql
CREATE TABLE employees (
    id NUMBER PRIMARY KEY,
    name VARCHAR2(100),
    department VARCHAR2(100),
    salary NUMBER
);
```

### **🔹 3️⃣ Insert Data**
```sql
INSERT INTO employees VALUES (1, 'Alice', 'HR', 5000);
INSERT INTO employees VALUES (2, 'Bob', 'IT', 6000);
```

### **🔹 4️⃣ Retrieve Data**
```sql
SELECT * FROM employees;
```

### **🔹 5️⃣ Update a Record**
```sql
UPDATE employees SET salary = 7000 WHERE id = 1;
```

### **🔹 6️⃣ Delete a Record**
```sql
DELETE FROM employees WHERE id = 2;
```

### **🔹 7️⃣ Drop Table**
```sql
DROP TABLE employees;
```

---

## **📢 Why This Setup is Better Than Local Installation?**
- **No need to install Oracle Database manually.**  
- **Avoid OS compatibility issues** (Windows EXE, missing `.deb` for Ubuntu, etc.).  
- **Access from any browser—no heavy system load.**  
- **Free cloud-based storage & auto-updates.**  

Instead of struggling with installation, simply log in and start coding SQL! 🚀  

---

## **📎 Resources & Documentation**
- **Oracle APEX Website:** [https://apex.oracle.com](https://apex.oracle.com)  
- **Official Documentation:** [https://docs.oracle.com/en/database/oracle/apex](https://docs.oracle.com/en/database/oracle/apex)  
- **Oracle Cloud Free Tier:** [https://www.oracle.com/cloud/free/](https://www.oracle.com/cloud/free/)  

---
