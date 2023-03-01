# Persistent-Cross-Site-Scripting-found-in-Online-Jewellery-Store-from-Sourcecodester-website.

Description: Persistent Cross Site Scripting leads to Cookie Stealing in Online Jewellery Store from Sourcecodester website.

[Additional Information] Persistent Cross Site scripting is a dangerous attack and in this scenario cookie stealing was possible through Cross Site Scripting (XSS). User input was trusted by the application and there was no escaping/filtering for the user inout which led to the XSS.

[Vulnerability Type] Cross Site Scripting (XSS)

[Vendor of Product] https://www.sourcecodester.com/

[Affected Product Code Base] Online Jewelry Shop using PHP/MySQLi with Source Code

[Affected Component] http://localhost/jewelry/admin/index.php?page=category_list

[Attack Type] Remote

[Impact Information Disclosure] True

[Attack Vectors] Steps to reproduce: 
Go to url http://localhost/jewelry/admin/index.php?page=category_list 
Click on "Categories" in the left column and click on "Add new"
Enter the payload "<script>alert(document.cookie)</script>" without double quotes in the "Category Name" field 
Click on "Save" 
XSS will be triggered and pop up with session cookie details appears.

[Discoverer] M Lohith

[LinkedIn] https://www.linkedin.com/in/lohithsai/
