# URLEncoder
using System;
using System.Collections.Generic;
using Stystem.Text

namespace Encoder
{
  Class Program
  {
      static void Main(string[] agrs)
      {
          Dictionary<char, string> substitue = new Dictionary<char, string>()
          {
              
              {'>', "%3E"},
              {'<', "%3C"},
              {'#', "%23"},
              {'%', "%25"},
              {'"', "%22"},
              
              {' ', "%20"},
              {';', "%3B"},
              {'/', "%2F"},
              {'?', "%3F"},
              {':', "%3A"},
              {'@', "%40"},
              {'&', "%26"},
              {'=', "%3D"},
              {'+', "%2B"},
              {'$', "%24"},
              {',', "%2C"},
              
              {'{', "%7B"},
              {'}', "%7D"},
              {'|', "%7C"},
              {'\\', "%5C"},
              {'^', "%5E"},
              {'[', "%5B"},
              {']', "%5D"},
              {'`', "%60"}
              
              
          };
          
          Console.WriteLine("Whats the name of your project:");
          string name = Console.ReadLine();
          Console.WriteLine("\nWrite the activity name:");
          string Activity = Console.Readline();
          
          
          StringBuilder converteName = new Stringbuilder();
          foreach(char c in project)
          {
          
              if(substitute.ContainsKey(C))
              {
                  convertedActivity.Append(substitute[c]);
              }
              else
              {
                  convertedName.Append(c);
              }
          }
          
          Console.WriteLine("\nYour encoded URL is: \nhttps://companyserver.com/content/{0}/files/{1}/{1}Report.pdf", convertedName, convertedActivity);

          
      }
  }
}
