//Trabalho de Logica de programação
// Alunos Kleber Alvares, Larryssa Araujo, Mateus Donaire,
// Thiago Marchi.
// RA 21304275, 21310055, 21286869,21289253.

package JDV;

import java.awt.Color;
import javax.swing.JFrame;
import javax.swing.JOptionPane;

public class JogoDaVelha_J extends javax.swing.JFrame {
    
    private String startGame="X";
    private int xCount = 0;
    private int oCount = 0;

    
    public JogoDaVelha_J() {
        initComponents();
        setSize(1200,600);
        setLocationRelativeTo(null);
        
    }

    private void gameScore()
    {
        jblPlayerX.setText(String.valueOf(xCount));
        jblPlayerO.setText(String.valueOf(oCount));
        if (xCount==3){
            xCount = 0;
            oCount = 0;
            jblPlayerX.setText("0");
            jblPlayerO.setText("0");
            JOptionPane.showMessageDialog(null,"Jogador X ganhou 3 vezes !!");
        }else if (oCount==3){
            oCount = 0;
            xCount = 0;
            jblPlayerX.setText("0");
            jblPlayerO.setText("0");
            JOptionPane.showMessageDialog(null,"Jogador O ganhou 3 vezes !!");

        }
    }
         
    private void choose_a_Player()
    {
        if (startGame.equalsIgnoreCase("X"))
        {
            startGame = "O";
        }
        else
        {
            startGame = "X";
        }
    }
    
    private void winningGame()
    {
        String b1 = jButton1.getText();
        String b2 = jButton2.getText();
        String b3 = jButton3.getText();
        
        String b4 = jButton4.getText();
        String b5 = jButton5.getText();
        String b6 = jButton6.getText();
        
        String b7 = jButton7.getText();
        String b8 = jButton8.getText();
        String b9 = jButton9.getText();
        
        if (b1== ("X") && b2 == ("X") && b3 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton1.setBackground(Color.GREEN);
            jButton2.setBackground(Color.GREEN);
            jButton3.setBackground(Color.GREEN);
            
            
            
        }
        if (b4== ("X") && b5 == ("X") && b6 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton4.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton6.setBackground(Color.GREEN);
        }
         if (b7== ("X") && b8 == ("X") && b9 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton7.setBackground(Color.GREEN);
            jButton8.setBackground(Color.GREEN);
            jButton9.setBackground(Color.GREEN);
        }
           if (b1== ("O") && b2 == ("O") && b3 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton1.setBackground(Color.GREEN);
            jButton2.setBackground(Color.GREEN);
            jButton3.setBackground(Color.GREEN);
        }
        if (b4== ("O") && b5 == ("O") && b6 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton4.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton6.setBackground(Color.GREEN);
        }
         if (b7== ("O") && b8 == ("O") && b9 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton7.setBackground(Color.GREEN);
            jButton8.setBackground(Color.GREEN);
            jButton9.setBackground(Color.GREEN);
        }
                 if (b1== ("X") && b5 == ("X") && b9 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton1.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton9.setBackground(Color.GREEN);
        }
        if (b1== ("O") && b5 == ("O") && b9 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton1.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton9.setBackground(Color.GREEN);
        }
                if (b3== ("X") && b5 == ("X") && b7 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton3.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton7.setBackground(Color.GREEN);
        }
        if (b3== ("O") && b5 == ("O") && b7 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton3.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton7.setBackground(Color.GREEN);
        }
                if (b1== ("X") && b4 == ("X") && b7 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton1.setBackground(Color.GREEN);
            jButton4.setBackground(Color.GREEN);
            jButton7.setBackground(Color.GREEN);
        }
        if (b1== ("O") && b4 == ("O") && b7 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton1.setBackground(Color.GREEN);
            jButton4.setBackground(Color.GREEN);
            jButton7.setBackground(Color.GREEN);
        }
                        if (b2== ("X") && b5 == ("X") && b8 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton2.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton8.setBackground(Color.GREEN);
        }
        if (b2== ("O") && b5 == ("O") && b8 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton2.setBackground(Color.GREEN);
            jButton5.setBackground(Color.GREEN);
            jButton8.setBackground(Color.GREEN);
        }
                        if (b3== ("X") && b6 == ("X") && b9 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'X' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            xCount++;
            gameScore();
            jButton3.setBackground(Color.GREEN);
            jButton6.setBackground(Color.GREEN);
            jButton9.setBackground(Color.GREEN);
        }
        if (b3== ("O") && b6 == ("O") && b9 == ("O"))
        {
            JOptionPane.showMessageDialog(this,"Jogador 'O' GANHOU !!"," Jogo da Velha",JOptionPane.INFORMATION_MESSAGE);
            oCount++;
            gameScore();
            jButton3.setBackground(Color.GREEN);
            jButton6.setBackground(Color.GREEN);
            jButton9.setBackground(Color.GREEN);
        }
       
    }
            
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">//GEN-BEGIN:initComponents
    private void initComponents() {

        jColorChooser1 = new javax.swing.JColorChooser();
        jColorChooser2 = new javax.swing.JColorChooser();
        jColorChooser3 = new javax.swing.JColorChooser();
        jColorChooser4 = new javax.swing.JColorChooser();
        jPanel1 = new javax.swing.JPanel();
        jLabel2 = new javax.swing.JLabel();
        jPanel3 = new javax.swing.JPanel();
        jPanel2 = new javax.swing.JPanel();
        jButton1 = new javax.swing.JButton();
        jPanel4 = new javax.swing.JPanel();
        jButton2 = new javax.swing.JButton();
        jPanel5 = new javax.swing.JPanel();
        jButton3 = new javax.swing.JButton();
        jPanel6 = new javax.swing.JPanel();
        jLabel1 = new javax.swing.JLabel();
        jPanel7 = new javax.swing.JPanel();
        jblPlayerX = new javax.swing.JLabel();
        jPanel8 = new javax.swing.JPanel();
        jButton4 = new javax.swing.JButton();
        jPanel9 = new javax.swing.JPanel();
        jButton5 = new javax.swing.JButton();
        jPanel10 = new javax.swing.JPanel();
        jButton6 = new javax.swing.JButton();
        jPanel11 = new javax.swing.JPanel();
        jLabel4 = new javax.swing.JLabel();
        jPanel12 = new javax.swing.JPanel();
        jblPlayerO = new javax.swing.JLabel();
        jPanel13 = new javax.swing.JPanel();
        jButton7 = new javax.swing.JButton();
        jPanel14 = new javax.swing.JPanel();
        jButton8 = new javax.swing.JButton();
        jPanel15 = new javax.swing.JPanel();
        jButton9 = new javax.swing.JButton();
        jPanel16 = new javax.swing.JPanel();
        jbnRec = new javax.swing.JButton();
        jPanel17 = new javax.swing.JPanel();
        jbnSair = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setBackground(new java.awt.Color(102, 102, 102));

        jPanel1.setForeground(new java.awt.Color(51, 51, 51));
        jPanel1.setLayout(new java.awt.BorderLayout());

        jLabel2.setFont(new java.awt.Font("Keep Calm Med", 0, 48)); // NOI18N
        jLabel2.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jLabel2.setText("Jogo da Velha");
        jPanel1.add(jLabel2, java.awt.BorderLayout.PAGE_START);

        jPanel3.setLayout(new java.awt.GridLayout(3, 5, 2, 2));

        jPanel2.setBackground(new java.awt.Color(51, 51, 51));
        jPanel2.setLayout(new java.awt.BorderLayout());

        jButton1.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton1.setForeground(new java.awt.Color(51, 51, 51));
        jButton1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton1ActionPerformed(evt);
            }
        });
        jPanel2.add(jButton1, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel2);

        jPanel4.setBackground(new java.awt.Color(51, 51, 51));
        jPanel4.setLayout(new java.awt.BorderLayout());

        jButton2.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton2.setForeground(new java.awt.Color(51, 51, 51));
        jButton2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton2ActionPerformed(evt);
            }
        });
        jPanel4.add(jButton2, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel4);

        jPanel5.setBackground(new java.awt.Color(51, 51, 51));
        jPanel5.setLayout(new java.awt.BorderLayout());

        jButton3.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton3.setForeground(new java.awt.Color(51, 51, 51));
        jButton3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton3ActionPerformed(evt);
            }
        });
        jPanel5.add(jButton3, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel5);

        jPanel6.setBackground(new java.awt.Color(51, 51, 51));
        jPanel6.setLayout(new java.awt.BorderLayout());

        jLabel1.setFont(new java.awt.Font("Keep Calm Med", 2, 36)); // NOI18N
        jLabel1.setForeground(new java.awt.Color(255, 255, 255));
        jLabel1.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jLabel1.setText("Jogador X ");
        jPanel6.add(jLabel1, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel6);

        jPanel7.setBackground(new java.awt.Color(51, 51, 51));
        jPanel7.setLayout(new java.awt.BorderLayout());

        jblPlayerX.setFont(new java.awt.Font("Keep Calm Med", 2, 48)); // NOI18N
        jblPlayerX.setForeground(new java.awt.Color(255, 255, 255));
        jblPlayerX.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jblPlayerX.setText("0");
        jPanel7.add(jblPlayerX, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel7);

        jPanel8.setBackground(new java.awt.Color(51, 51, 51));
        jPanel8.setLayout(new java.awt.BorderLayout());

        jButton4.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton4.setForeground(new java.awt.Color(51, 51, 51));
        jButton4.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton4ActionPerformed(evt);
            }
        });
        jPanel8.add(jButton4, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel8);

        jPanel9.setBackground(new java.awt.Color(51, 51, 51));
        jPanel9.setLayout(new java.awt.BorderLayout());

        jButton5.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton5.setForeground(new java.awt.Color(51, 51, 51));
        jButton5.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton5ActionPerformed(evt);
            }
        });
        jPanel9.add(jButton5, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel9);

        jPanel10.setBackground(new java.awt.Color(51, 51, 51));
        jPanel10.setLayout(new java.awt.BorderLayout());

        jButton6.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton6.setForeground(new java.awt.Color(51, 51, 51));
        jButton6.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton6ActionPerformed(evt);
            }
        });
        jPanel10.add(jButton6, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel10);

        jPanel11.setBackground(new java.awt.Color(51, 51, 51));
        jPanel11.setLayout(new java.awt.BorderLayout());

        jLabel4.setFont(new java.awt.Font("Keep Calm Med", 2, 36)); // NOI18N
        jLabel4.setForeground(new java.awt.Color(255, 255, 255));
        jLabel4.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jLabel4.setText("Jogador O");
        jPanel11.add(jLabel4, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel11);

        jPanel12.setBackground(new java.awt.Color(51, 51, 51));
        jPanel12.setLayout(new java.awt.BorderLayout());

        jblPlayerO.setFont(new java.awt.Font("Keep Calm Med", 2, 48)); // NOI18N
        jblPlayerO.setForeground(new java.awt.Color(255, 255, 255));
        jblPlayerO.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jblPlayerO.setText("0");
        jPanel12.add(jblPlayerO, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel12);

        jPanel13.setBackground(new java.awt.Color(51, 51, 51));
        jPanel13.setLayout(new java.awt.BorderLayout());

        jButton7.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton7.setForeground(new java.awt.Color(51, 51, 51));
        jButton7.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton7ActionPerformed(evt);
            }
        });
        jPanel13.add(jButton7, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel13);

        jPanel14.setBackground(new java.awt.Color(51, 51, 51));
        jPanel14.setLayout(new java.awt.BorderLayout());

        jButton8.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton8.setForeground(new java.awt.Color(51, 51, 51));
        jButton8.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton8ActionPerformed(evt);
            }
        });
        jPanel14.add(jButton8, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel14);

        jPanel15.setBackground(new java.awt.Color(51, 51, 51));
        jPanel15.setLayout(new java.awt.BorderLayout());

        jButton9.setFont(new java.awt.Font("Keep Calm Med", 1, 96)); // NOI18N
        jButton9.setForeground(new java.awt.Color(51, 51, 51));
        jButton9.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton9ActionPerformed(evt);
            }
        });
        jPanel15.add(jButton9, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel15);

        jPanel16.setBackground(new java.awt.Color(51, 51, 51));
        jPanel16.setLayout(new java.awt.BorderLayout());

        jbnRec.setFont(new java.awt.Font("Keep Calm Med", 0, 20)); // NOI18N
        jbnRec.setForeground(new java.awt.Color(51, 51, 51));
        jbnRec.setText("Jogar Novamente");
        jbnRec.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbnRecActionPerformed(evt);
            }
        });
        jPanel16.add(jbnRec, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel16);

        jPanel17.setBackground(new java.awt.Color(51, 51, 51));
        jPanel17.setLayout(new java.awt.BorderLayout());

        jbnSair.setFont(new java.awt.Font("Keep Calm Med", 0, 24)); // NOI18N
        jbnSair.setForeground(new java.awt.Color(51, 51, 51));
        jbnSair.setText("Sair");
        jbnSair.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbnSairActionPerformed(evt);
            }
        });
        jPanel17.add(jbnSair, java.awt.BorderLayout.CENTER);

        jPanel3.add(jPanel17);

        jPanel1.add(jPanel3, java.awt.BorderLayout.CENTER);

        getContentPane().add(jPanel1, java.awt.BorderLayout.CENTER);

        pack();
    }// </editor-fold>//GEN-END:initComponents
private JFrame frame;

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton1ActionPerformed

    jButton1.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton1.setForeground(Color.BLACK);
        }
        else
        {
             jButton1.setForeground(Color.BLACK);
        }
        choose_a_Player();
         winningGame();
         
        
    }//GEN-LAST:event_jButton1ActionPerformed

    private void jbnSairActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jbnSairActionPerformed
        // TODO add your handling code here:       frame = new JFrame("Sair");
       if (JOptionPane.showConfirmDialog(frame,"Clique em 'Sim' para sair ","Jogo da Velha",
               JOptionPane.YES_NO_OPTION)== JOptionPane.YES_NO_OPTION)
       {
           System.exit(0);
       }                
       else 
       {
        
               }

    }//GEN-LAST:event_jbnSairActionPerformed

    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton2ActionPerformed
       
        jButton2.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton2.setForeground(Color.BLACK);
        }
        else
        {
             jButton2.setForeground(Color.BLACK);
        }
        choose_a_Player();
         winningGame();
         
    }//GEN-LAST:event_jButton2ActionPerformed

    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton3ActionPerformed

          jButton3.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton3.setForeground(Color.BLACK);
        }
        else
        {
             jButton3.setForeground(Color.BLACK);
        }
        choose_a_Player();
         winningGame();
        
    }//GEN-LAST:event_jButton3ActionPerformed

    private void jButton6ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton6ActionPerformed

  jButton6.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton6.setForeground(Color.BLACK);
        }
        else
        {
             jButton6.setForeground(Color.BLACK);
        }
        choose_a_Player();
               winningGame();
       
    }//GEN-LAST:event_jButton6ActionPerformed

    private void jButton5ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton5ActionPerformed

     jButton5.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton5.setForeground(Color.BLACK);
        }
        else
        {
             jButton5.setForeground(Color.BLACK);
        }
        choose_a_Player();
               winningGame();
    }//GEN-LAST:event_jButton5ActionPerformed

    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton4ActionPerformed
    
          jButton4.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton4.setForeground(Color.BLACK);
        }
        else
        {
             jButton4.setForeground(Color.BLACK);
        }
        choose_a_Player();
               winningGame();
    }//GEN-LAST:event_jButton4ActionPerformed

    private void jButton9ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton9ActionPerformed

        jButton9.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton9.setForeground(Color.BLACK);
        }
        else
        {
             jButton9.setForeground(Color.BLACK);
        }
        choose_a_Player();
               winningGame();
    }//GEN-LAST:event_jButton9ActionPerformed

    private void jButton8ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton8ActionPerformed
          jButton8.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton8.setForeground(Color.BLACK);
        }
        else
        {
             jButton8.setForeground(Color.BLACK);
        }
        choose_a_Player();
               winningGame();
    }//GEN-LAST:event_jButton8ActionPerformed

    private void jButton7ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton7ActionPerformed
         jButton7.setText(startGame);
        
        if (startGame.equalsIgnoreCase("X"))
        {
            jButton7.setForeground(Color.BLACK);
        }
        else
        {
             jButton7.setForeground(Color.BLACK);
        }
        choose_a_Player();
               winningGame();
    }//GEN-LAST:event_jButton7ActionPerformed

    private void jbnRecActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jbnRecActionPerformed
   jButton1.setText(null);
    jButton2.setText(null);
     jButton3.setText(null);
      jButton4.setText(null);
       jButton5.setText(null);
        jButton6.setText(null);
         jButton7.setText(null);
          jButton8.setText(null);
           jButton9.setText(null);
           
   jButton1.setBackground(Color.LIGHT_GRAY) ; 
   jButton2.setBackground(Color.LIGHT_GRAY) ;      
   jButton3.setBackground(Color.LIGHT_GRAY) ;      
   jButton4.setBackground(Color.LIGHT_GRAY) ;      
   jButton5.setBackground(Color.LIGHT_GRAY) ;      
   jButton6.setBackground(Color.LIGHT_GRAY) ;      
   jButton7.setBackground(Color.LIGHT_GRAY) ;      
   jButton8.setBackground(Color.LIGHT_GRAY) ;      
   jButton9.setBackground(Color.LIGHT_GRAY) ;      
   
   
           
        
   
    }//GEN-LAST:event_jbnRecActionPerformed

    public static void main(String args[]) {

        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new JogoDaVelha_J().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify//GEN-BEGIN:variables
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JButton jButton4;
    private javax.swing.JButton jButton5;
    private javax.swing.JButton jButton6;
    private javax.swing.JButton jButton7;
    private javax.swing.JButton jButton8;
    private javax.swing.JButton jButton9;
    private javax.swing.JColorChooser jColorChooser1;
    private javax.swing.JColorChooser jColorChooser2;
    private javax.swing.JColorChooser jColorChooser3;
    private javax.swing.JColorChooser jColorChooser4;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel jLabel4;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JPanel jPanel10;
    private javax.swing.JPanel jPanel11;
    private javax.swing.JPanel jPanel12;
    private javax.swing.JPanel jPanel13;
    private javax.swing.JPanel jPanel14;
    private javax.swing.JPanel jPanel15;
    private javax.swing.JPanel jPanel16;
    private javax.swing.JPanel jPanel17;
    private javax.swing.JPanel jPanel2;
    private javax.swing.JPanel jPanel3;
    private javax.swing.JPanel jPanel4;
    private javax.swing.JPanel jPanel5;
    private javax.swing.JPanel jPanel6;
    private javax.swing.JPanel jPanel7;
    private javax.swing.JPanel jPanel8;
    private javax.swing.JPanel jPanel9;
    private javax.swing.JLabel jblPlayerO;
    private javax.swing.JLabel jblPlayerX;
    private javax.swing.JButton jbnRec;
    private javax.swing.JButton jbnSair;
    // End of variables declaration//GEN-END:variables
}
// Código inpirado em DJ Oamen
// vídeo :https://www.youtube.com/watch?v=nOyPmAVtceQ
