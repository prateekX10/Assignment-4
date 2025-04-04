# Asignment - 4
#TASK - 1

# IF FILE EXISTS

try:
  
  file1 = open("sample.txt", "r+")
  read_file = file1.read()
  print(read_file)
  file1.close()
  
except FileNotFoundError:
  print("Error: The file 'sample.txt' was not found")



#TASK - 2
file2 = open("output.txt", "r+")
write_file  = file2.write(input("Enter text to write to the file: "))
print("Data successfully written in file output.txt\n")
file2.close()

file2 = open("output.txt", "a")
append_file = file2.write("\n" + input("Enter text to append to the file: "))
print("Data successfully appended\n")
file2.close()

file2 = open("output.txt", "r+")
read_file = file2.read()
print("Final context of output.txt\n")
print(read_file)
file2.close()

