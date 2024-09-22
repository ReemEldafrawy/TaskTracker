https://roadmap.sh/projects/task-tracker
using static System.Net.Mime.MediaTypeNames;
using System.Collections.Generic;
using System.IO;
using System.Reflection.Metadata;
using System.Runtime.Intrinsics.X86;
using System.Threading.Tasks;
using System;

namespace TaskTracker
{
    

    public class program
    {
       
        public static void Main(string[] args)
        {
            Console.WriteLine("Welcome to you");
            TaskManager task = new TaskManager();
            while (true)
            { 
                Console.WriteLine("Enter Your Choice From 1 To 5");
                Console.WriteLine("1. Add a task");
                Console.WriteLine("2. View all tasks");
                Console.WriteLine("3. Mark a task as completed");
                Console.WriteLine("4. Remove a task");
                Console.WriteLine("5. Exit");

                string ChoiceJop = Console.ReadLine();
                switch (ChoiceJop)
                {
                    case "1":
                        //Add tasks
                        task.AddTasks();
                        break;
                    case "2":
                        //View all tasks
                        task.ViewTasks();
                        break;
                    case "3":
                        //mark task completed
                        task.MarKTasksCompleted();
                        break;
                    case "4":
                        //Remove task
                        task.RemoveTask();
                        break;
                    case "5":
                        //Exit
                        task.Exit();
                        return;
                    default:
                        Console.WriteLine("Enter number from 1 to 5 only");
                        break;
                }
            }
        }
        
      














    }
}
