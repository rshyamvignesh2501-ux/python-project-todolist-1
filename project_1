do_list=[]

def menu():
    while(True):
        print("**MAIN MENU**")
        print("1.Add a new task")
        print("2.View the task")
        print("3.Remove the task")
        print("4.Mark the status")
        print("5.Exit")

        choice=input("enter your choice")
        if choice=="1":
            add_task()
        elif choice=="2":
            view_task()
        elif choice=="3":
            remove_task()
        elif choice=="4":
            mark_done()
        elif choice=="5":
            exit()
    
def add_task():
    task=input("enter the task ")
    do_list.append({"Task":task,"Status":"pending"})
    print(f"task added successfully \n")

    
def view_task():
    print("your do list:")
    if len(do_list)==0:
        print("no tasks has been added")
    else:
        for index,task in enumerate(do_list,1):
            print(f"{index},{task['Task']}-{task['Status']}")
            print("\n")

            
def remove_task():
    if len(do_list)==0:
        print("list is empty")
    else:
        try:
            search=int(input("enter the task number:"))-1
            if 0<= search <len(do_list):
                removed=do_list.pop(search)
                print(f"task removed,{removed['Task']}")
            else:
                print("invalid number, please try again")
        except ValueError:
            print("please add a valid number:")

            
def mark_done():
    if len(do_list)==0:
        print("list is empty")
    else:
            search=int(input("enter the task number that you want to mark as done"))-1
            if 0<= search <len(do_list):
                do_list[search]['status']='done'
                print(f"Task {do_list[search]['Task']}has been marked as done")
            else:
                print("invalid number, please try again")
menu()
            
            


            
        
    
