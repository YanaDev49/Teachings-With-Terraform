# What does terraform plan do? 🤔

![image](https://github.com/user-attachments/assets/a7b5f39f-0635-45b8-845a-16b7fbdcfac3)

### The command terraform plan allows you to see what your changes will do.

Terraform analyses your configuration files, compares them to the current state of your infrastructure and then generates a plan  

### essentially, terraform plan is like a preview of what Terraform is going to do. It checks your code and shows you what changes it’s about to make to your infrastructure before actually doing anything. It's a safe way to see what will happen without making any changes yet.

## What Happens When You Run terraform plan:
  
𝗖𝗵𝗲𝗰𝗸𝘀 𝘁𝗵𝗲 𝗰𝗼𝗱𝗲: Terraform looks at your configuration (the .tf files you wrote) to see what resources you want to create, update, or delete.
##
𝗖𝗼𝗺𝗽𝗮𝗿𝗲𝘀 𝘄𝗶𝘁𝗵 𝘁𝗵𝗲 𝗰𝘂𝗿𝗿𝗲𝗻𝘁 𝘀𝘁𝗮𝘁𝗲: It checks what already exists in your cloud provider (like AWS) by comparing with your state file (a file that tracks your existing infrastructure).
##
𝗦𝗵𝗼𝘄𝘀 𝘆𝗼𝘂 𝘁𝗵𝗲 𝗽𝗹𝗮𝗻: Terraform then gives you a "plan" — listing what it’s going to create, update, or delete. 


<img width="650" alt="Screenshot 2024-10-16 170610" src="https://github.com/user-attachments/assets/f174f5f0-4ebc-42a3-ada7-2ed584d5c8fb">


![Screenshot 2024-10-16 171231](https://github.com/user-attachments/assets/d542088e-4b16-449d-bd15-9aea33d0fbf8)

#### - '+' for resources that will be added (new ones).
  
#### - ~ for resources that will be modified (changed settings).

#### - '-' for resources that will be deleted.

## A further breakdown

### When you run terraform plan, Terraform is basically checking the current state of your infrastructure against the desired state that you've defined in your configuration files.

Current state: This is what your infrastructure looks like right now, based on what’s already been created or modified. Terraform keeps track of this in a state file (like terraform.tfstate), which holds details about the resources it’s managing.

Desired state: This is what you're aiming for—what you've written in your .tf files. These files define the resources you need, how they should be configured, and how they should connect.

### When you run terraform plan, it:

- Looks at the current state to see what’s already in place.
- Compares that to the desired state you’ve defined in your code.
- Shows you a plan of what changes will be made—whether it needs to create, update, or delete resources to get your infrastructure to match what you've described.

![ThereYouHaveItSheaWhitneyGIF (2)](https://github.com/user-attachments/assets/17b7a5d4-f63b-476c-ae80-243732c086cb)
