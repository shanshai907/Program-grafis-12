<img width="300" height="143" alt="Screenshot 2026-01-30 094037" src="https://github.com/user-attachments/assets/4c881066-f223-49c4-a95d-6ef0a792d9be" />


import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class input_data extends javax.swing.JFrame {

    
    public input_data() {
        initComponents();
    }

   
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        jLabel1 = new javax.swing.JLabel();
        jTextField1 = new javax.swing.JTextField();
        jButton1 = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        jLabel1.setText("jLabel1");

        jTextField1.setText("jTextField1");

        jButton1.setText("jButton1");

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                    .addComponent(jButton1)
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                        .addGroup(layout.createSequentialGroup()
                            .addGap(176, 176, 176)
                            .addComponent(jLabel1))
                        .addGroup(layout.createSequentialGroup()
                            .addGap(162, 162, 162)
                            .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))))
                .addContainerGap(167, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGap(72, 72, 72)
                .addComponent(jLabel1)
                .addGap(42, 42, 42)
                .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, 67, Short.MAX_VALUE)
                .addComponent(jButton1)
                .addGap(58, 58, 58))
        );

        pack();
    }// </editor-fold>                        

    
    public static void main(String args[]) {
       
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                  // Membuat frame
        JFrame frame = new JFrame("Form Input Nama");
        frame.setSize(300, 150);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setLayout(null);

        // Membuat label
        JLabel label = new JLabel("Masukkan Nama:");
        label.setBounds(20, 20, 120, 20);
        frame.add(label);

        // Membuat text field
        JTextField textField = new JTextField();
        textField.setBounds(140, 20, 120, 20);
        frame.add(textField);

        // Membuat button
        JButton button = new JButton("Submit");
        button.setBounds(100, 60, 80, 30);
        frame.add(button);

        // Menambahkan action listener untuk button
        button.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                String nama = textField.getText();
                JOptionPane.showMessageDialog(frame, "Halo, " + nama + "!");
            }
        });

        // Menampilkan frame
        frame.setVisible(true);
    }
            
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton jButton1;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JTextField jTextField1;
    // End of variables declaration                   
}

