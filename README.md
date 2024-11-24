# CS4Q2PE1
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

public class cs4q2pe1 {
    JFrame frame;
    JLabel console;
    JButton m;
    JButton p;
    JButton l;
    JButton lstick;
    JButton rstick;
    JButton u;
    JButton r;
    JButton d;
    JButton b;
    
    JButton u2;
    JButton r2;
    JButton d2;
    JButton b2;
    JButton l2;
    
    JTextArea screen;
    
    public cs4q2pe1() {
        frame=new JFrame("CS4Q2PE1");
        console = new JLabel("Game Console");
        screen = new JTextArea();
        
        m = new JButton("M");
        lstick = new JButton("LStick");
        u = new JButton("U");
        l = new JButton("L");
        r = new JButton("R");
        d = new JButton("D");
        b = new JButton("B");
        
        p = new JButton("P");
        rstick = new JButton("RStick");
        u2 = new JButton("U");
        l2 = new JButton("L");
        r2 = new JButton("R");
        d2 = new JButton("D");
        b2 = new JButton("B");
    }
    
    public void setFrame() {
         frame.setLayout(new GraphPaperLayout(new Dimension(26,13)));
         
         frame.add(screen, new Rectangle(5,3,15,9));
         frame.add(console, new Rectangle(5,1,15,1));
         
         frame.add(m, new Rectangle(3,1,1,1));
         frame.add(l, new Rectangle(1,8,1,1));
         frame.add(u, new Rectangle(2,7,1,1));
         frame.add(r, new Rectangle(3,8,1,1));
         frame.add(d, new Rectangle(2,9,1,1));
         frame.add(b, new Rectangle(3,11,1,1));

         frame.add(p, new Rectangle(22,1,1,1));
         frame.add(l2, new Rectangle(22,4,1,1));
         frame.add(u2, new Rectangle(23,3,1,1));
         frame.add(r2, new Rectangle(24,4,1,1));
         frame.add(d2, new Rectangle(23,5,1,1));
         frame.add(b2, new Rectangle(22,11,1,1));
         
        frame.add(rstick, new Rectangle(23,8,2,2));
        frame.add(lstick, new Rectangle(1,3,2,2));
         
        frame.setVisible(true);
        frame.setDefaultCloseOperation(frame.DISPOSE_ON_CLOSE);
        frame.setSize(1200,500);
    }
    
    public static void main(String[] args) {
        cs4q2pe1 gconsole = new cs4q2pe1();
        gconsole.setFrame();
    }
}

