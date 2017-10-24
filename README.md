package component;

import javax.swing.JOptionPane;

public class PlaneCoordinates

{
    
    public static void main (String args[])
     {
         String input1, input2, input3, input4, results1, results2, results3, results4="";
         int  x1,y1,x2,y2;
         double distance,midpoint1,midpoint2,slope;
         
         input1=JOptionPane.showInputDialog("Enter point on plane for x1");
         input2=JOptionPane.showInputDialog("Enter point on plane for y1");
         input3=JOptionPane.showInputDialog("Enter point on plane for x2");
         input4=JOptionPane.showInputDialog("Enter point on plane for y2"); 
         
         x1=Integer.parseInt(input1);
         y1=Integer.parseInt(input2);
         x2=Integer.parseInt(input3);
         y2=Integer.parseInt(input4);
         
         distance=(Math.sqrt(((x2-x1)^2) + ((y2-y1)^2)));
         midpoint1=(x1+x2)/2.0;
         midpoint2=((y1+y2)/2);
         slope=(y2-y1)/(x2-x1);
         
         results1="Distance between points: d= "+distance;
         results2="Midpoint (x',y') with x' = "+midpoint1;
         results3="Midpoint (x',y') with y' = "+midpoint2;
         results4="The slope of the line is = "+slope;
         
          JOptionPane.showMessageDialog(null,results1,"PlaneCoordiantes",JOptionPane.INFORMATION_MESSAGE);
          JOptionPane.showMessageDialog(null,results2,"PlaneCoordiantes",JOptionPane.INFORMATION_MESSAGE);
          JOptionPane.showMessageDialog(null,results3,"PlaneCoordiantes",JOptionPane.INFORMATION_MESSAGE);
          JOptionPane.showMessageDialog(null,results4,"PlaneCoordiantes",JOptionPane.INFORMATION_MESSAGE);


     }
     
}

