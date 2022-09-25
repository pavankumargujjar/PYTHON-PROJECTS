from tkinter import *
import datetime
import time
import winsound

def alarm(set_alarm_timer):
    while True:
        time.sleep(1)
        current_time = datetime.datetime.now()
        now = current_time.strftime("%H:%M:%S")
        date = current_time.strftime("%d/%m/%y")
        print("Today's date is = ",date)
        print("Current time is = ",now)
        if now == set_alarm_timer:
            print("Time to wake up")
            winsound.PlaySound("sound.wav",winsound.SND_ASYNC)

def actual_time():
    set_alarm_timer = f"{hour.get()}:{min.get()}:{sec.get()}"
    alarm(set_alarm_timer)

clock = Tk()
clock.title("Pavan's alarm clock")
clock.iconbitmap("alarm.ico")
clock.geometry("400x200")
time_format = Label(clock, text = "Enter the time in 24 hours format!", fg="red", bg="black", font="Arial").place(x=60, y=120)
addTime = Label(clock, text = "Hour, Min, Sec", font=60).place(x=110)
setYourAlarm = Label(clock, text = "When to wake you up", fg="blue", relief = "solid", font = ("Arial,7,bold")).place(x=0, y=29)


hour = StringVar()
min = StringVar()
sec = StringVar()

hourTime = Entry(clock, textvariable = hour, bg = "pink", width=15).place(x=180, y=30)
minTime = Entry(clock, textvariable = min, bg = "pink", width=15).place(x=220, y=30)
secTime = Entry(clock, textvariable = sec, bg = "pink", width=15).place(x=280, y=30)


submit = Button(clock, text = "Set Alarm", fg = "red", bg = "blue", width = 10, command = "actual_time").place(x=110, y=70)


clock.mainloop()
