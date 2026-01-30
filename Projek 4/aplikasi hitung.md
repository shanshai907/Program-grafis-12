<img width="348" height="195" alt="Screenshot 2026-01-30 094310" src="https://github.com/user-attachments/assets/63eee4d7-0d05-4098-8c12-7a523d066256" />


import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
public class aplikasi_hitung extends javax.swing.JFrame {

    
    public aplikasi_hitung() {
        initComponents();
    }

    
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        jTextField1 = new javax.swing.JTextField();
        jTextField2 = new javax.swing.JTextField();
        jButton1 = new javax.swing.JButton();
        jLabel1 = new javax.swing.JLabel();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        jTextField1.setText("jTextField1");

        jTextField2.setText("jTextField2");

        jButton1.setText("jButton1");

        jLabel1.setText("jLabel1");

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addGap(162, 162, 162)
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                            .addComponent(jButton1)
                            .addComponent(jTextField2, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)))
                    .addGroup(layout.createSequentialGroup()
                        .addGap(179, 179, 179)
                        .addComponent(jLabel1)))
                .addContainerGap(163, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGap(76, 76, 76)
                .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(18, 18, 18)
                .addComponent(jTextField2, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(34, 34, 34)
                .addComponent(jButton1)
                .addGap(41, 41, 41)
                .addComponent(jLabel1)
                .addContainerGap(48, Short.MAX_VALUE))
        );

        pack();
    }// </editor-fold>                        

    public static void main(String args[]) {
        
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                 // Membuat frame
        JFrame frame = new JFrame("Aplikasi Hitung Sederhana");
        frame.setSize(350, 200);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setLayout(null);

        // Membuat label dan text field untuk angka pertama
        JLabel labelAngka1 = new JLabel("Angka Pertama:");
        labelAngka1.setBounds(20, 20, 120, 20);
        frame.add(labelAngka1);

        JTextField textFieldAngka1 = new JTextField();
        textFieldAngka1.setBounds(140, 20, 150, 20);
        frame.add(textFieldAngka1);

        // Membuat label dan text field untuk angka kedua
        JLabel labelAngka2 = new JLabel("Angka Kedua:");
        labelAngka2.setBounds(20, 50, 120, 20);
        frame.add(labelAngka2);

        JTextField textFieldAngka2 = new JTextField();
        textFieldAngka2.setBounds(140, 50, 150, 20);
        frame.add(textFieldAngka2);

        // Membuat button untuk menghitung
        JButton buttonHitung = new JButton("Hitung");
        buttonHitung.setBounds(100, 90, 100, 30);
        frame.add(buttonHitung);

        // Membuat label untuk menampilkan hasil
        JLabel labelHasil = new JLabel("Hasil: ");
        labelHasil.setBounds(20, 130, 270, 20);
        frame.add(labelHasil);

        // Menambahkan action listener untuk button
        buttonHitung.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                try {
                    double angka1 = Double.parseDouble(textFieldAngka1.getText());
                    double angka2 = Double.parseDouble(textFieldAngka2.getText());
                    double hasil = angka1 + angka2;
                    labelHasil.setText("Hasil: " + angka1 + " + " + angka2 + " = " + hasil);
                } catch (NumberFormatException ex) {
                    JOptionPane.showMessageDialog(frame, "Masukkan angka yang valid!", "Error", JOptionPane.ERROR_MESSAGE);
                }
            }
        });

        // Menampilkan frame
        frame.setVisible(true);
    }


                //new aplikasi_hitung().setVisible(true);
            
        });
    
}

        
    

    // Variables declaration - do not modify                     
    private javax.swing.JButton jButton1;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JTextField jTextField1;
    private javax.swing.JTextField jTextField2;
    // End of variables declaration                   
}
