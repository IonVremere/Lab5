# Lab5

int d; // Number of days
// if the student is at least 18 years of age
if (student.Age> = 18)
{
    //invitation message directly to the student
    notificationService.SendMessageTo(student, meetingInvitation);
}
else // if the student is younger than 18 years 
{
    // invitation message to the person responsible for the student
    notificationService.SendMessageTo(student.Parent, meetingInvitation);
}
// student is eligible for blood donation
if (student.Age >= 17 && student.Weight >= 58.0 && student.Height >= 1.55)
{
    ScheduleBloodDonatingSessionWith(student);
}
