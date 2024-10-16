# What does terraform plan do? 🤔

![image](https://github.com/user-attachments/assets/a7b5f39f-0635-45b8-845a-16b7fbdcfac3)

### The command terraform plan allows you to see what your changes will do.

Terraform analyses your configuration files, compares them to the current state of your infrastructure and then generates a plan  

### essentially, terraform plan is like a preview of what Terraform is going to do. It checks your code and shows you what changes it’s about to make to your infrastructure before actually doing anything. It's a safe way to see what will happen without making any changes yet.

- What Happens When You Run terraform plan:
  
Checks the code: Terraform looks at your configuration (the .tf files you wrote) to see what resources you want to create, update, or delete.

Compares with the current state: It checks what already exists in your cloud provider (like AWS) by comparing with your state file (a file that tracks your existing infrastructure).

Shows you the plan: Terraform then gives you a "plan" — listing what it’s going to create, update, or delete. 


<img width="650" alt="Screenshot 2024-10-16 170610" src="https://github.com/user-attachments/assets/f174f5f0-4ebc-42a3-ada7-2ed584d5c8fb">


![Screenshot 2024-10-16 171231](https://github.com/user-attachments/assets/d542088e-4b16-449d-bd15-9aea33d0fbf8)

- '+' for resources that will be added (new ones).
  
- ~ for resources that will be modified (changed settings).

- '-' for resources that will be deleted.

![ThereYouHaveItSheaWhitneyGIF (2)](https://github.com/user-attachments/assets/17b7a5d4-f63b-476c-ae80-243732c086cb)
