import javax.swing.*;
import java.awt.*;

public class InvitationCard extends JFrame {

    public InvitationCard() {
        setTitle("Invitation Card");
        setSize(400, 300);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null);

        JPanel panel = new JPanel() {
            @Override
            protected void paintComponent(Graphics g) {
                super.paintComponent(g);
                g.setFont(new Font("Serif", Font.BOLD, 24));
                g.setColor(Color.RED);
                g.drawString("You're Invited!", 100, 50);

                g.setFont(new Font("Serif", Font.PLAIN, 18));
                g.setColor(Color.BLACK);
                g.drawString("Join us for a special event", 80, 100);
                g.drawString("Date: April 1, 2025", 120, 140);
                g.drawString("Time: 6:00 PM", 140, 180);
                g.drawString("Venue: Funoramoto's Place", 110, 220);
                g.drawstring("Play: Hello",220,240);
