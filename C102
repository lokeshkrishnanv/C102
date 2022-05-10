import dropbox as dbx

def main():
    name = input("Please Enter Your Name : ")
    phoneNo = input("Please Enter Your Phone Number : ")
    age = input("Please Enter Your Age : ")
    gender = input("Please Enter Your Gender : ")
    mother_name = input("Please Enter Your Mother Name : ")
    father_name = input("Please Enter Your Father Name : ")
    address = input("Please Enter Your Full Address : ")
    date_of_birth = input("Please Enter Your Date Of Birth : ")

    with open("info.txt", "w+") as f:
        f.writelines("Name : "+ str(name) + "\n")
        f.writelines("Phone No : "+ str(phoneNo) + "\n")
        f.writelines("Age : "+ str(age) + "\n")
        f.writelines("Gender : "+ str(gender) + "\n")
        f.writelines("Mother Name : "+ str(mother_name) + "\n")
        f.writelines("Father Name : "+ str(father_name) + "\n")
        f.writelines("Address : "+ str(address) + "\n")
        f.writelines("Date Of Birth : "+ str(date_of_birth) + "\n")
    
    file_from = "info.txt"
    file_to = input("Please Enter The Dropbox Path Where You Want To Upload This File : ")
    upload_files(file_from, file_to)

def upload_files(file_from, file_to):
    access_token = 'ACCESS_TOKEN'

    dbx = dropbox.Dropbox(self.access_token)

    with open(file_from, 'rb') as f:
        dbx.files_upload(f.read(), file_to)
    
    print("Your Data Has Been Uploaded To Dropbox Successfuly!")

main()
