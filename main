print("\n")
FSInput = str(input("Use mb\gb for file size ? : "))
DSFInput = str(input("Use kb\mb for download speed ? : "))
print("\n")

FileSize = float(input("Enter File Size In " + str(FSInput) + " : "))
DownloadSpeed = float(input("Enter Download Speed In " + str(DSFInput) + "\s : "))

DownloadETAs = (float(FileSize) * 1024 / float(DownloadSpeed))
DownloadETAm = (float(FileSize) * 1024 / float(DownloadSpeed) / 60)
DownloadETAh = (float(FileSize) * 1024 / float(DownloadSpeed) / 60 / 60)
print("\n")

print("File Size : " + str(FileSize) +" " + str(FSInput) + " || " + "Download Speed : " + str(DownloadSpeed) + " " + str(DSFInput) + "\s")
match FSInput:
    case "gb":
        FileSize = (float(FileSize) * 1024)
    case "mb":
        FileSize = FileSize
FSInput = ["gb", "mb"]
for x in FSInput:
    if x != ("mb" or "gb"):
        break

match DSFInput:
    case "mb":
        DownloadSpeed = (float(DownloadSpeed) * 1024)
    case "kb":
        DownloadSpeed = DownloadSpeed
DSInput = ["gb", "mb"]
for x in DSInput:
    if x != ("kb" or "mb"):
        break

print("Estimated Download Time : "+str(round(DownloadETAh, 2))+"-Hr | "+str(round(DownloadETAm, 1))+"-Min | "+str(round(DownloadETAs, 1))+"-Sec")
