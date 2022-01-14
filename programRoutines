import os, os.path

def fileSearchControl(file):
    #the program is intended to accept the name of a file
    #check if it CAN be the name of a file
    #and look for it inside all the directories of a computer
    #it will return the file if present
    #else an error message
    file = file.strip()
   ''' dir = os.getcwd()
   findFile(dir, search)
   
def findFile(dir, search) :
   if os.path.isdir(dir) :
      names = os.listdir(dir)
      for name in names :
         if os.path.isfile(dir + os.sep + name) :
            if search in name :
               print(dir + os.sep + name)
         else : # è una cartella
            findFile(dir + os.sep + name, search)   
    '''
    if file.startswith('https:\\') or file.startswith('http:\\'):
        with urlopen(file) as data:
            text = data.read().decode('utf-8')
    else:
        directory = input('Please input the path of the directory you wanna start your search, or write "parent" if you wanna start from scratch: ')
        directory = directory.strip()
        if directory.lower() == 'parent':
            directory = 'C:\\'
        elif directory == '':
            directory = os.getcwd()
        elif not os.isDir(directory):
            return 'Not a directory!'
        findFile(directory, file)
        

    
