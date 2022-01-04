package com.essamsalem.mohamed.mohamedtest;

import java.io.File;
import java.io.FileNotFoundException;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.FilterWriter;
import java.io.IOException;
import javax.swing.JOptionPane;

public class Main {

    public static void main(String[] args) {



        //Start do not edit
        FileReader fr = null;
        FileWriter fw = null;
        //End do not edit

        try {
            //the list of files folder path
            File fdis = new File("C:\\Users\\moham\\Desktop\\Test");
            //the list of files folder path
            
            //array that saves the files names
            File[] lstFile = fdis.listFiles();
            
            ///the loop that loops on the files one by one
            for (int i = 0; i < lstFile.length; i++) {
                String loopFileN = lstFile[i].getName();

                try {
                    
                    //the first folder path that you want to copy from
                    File f = new File("C:\\Users\\moham\\Desktop\\Test\\" + loopFileN);
                    fr = new FileReader(f);
                    //the second folder path that you want to paste to
                    fw = new FileWriter("C:\\Users\\moham\\Desktop\\Test2\\" + loopFileN);

                    int c = fr.read();
                    //the while loop that loops on the leters in the file and copy it one by one to the other file in the seconf folder
                    while (c != -1) {
                        System.out.print((char) c);
                        fw.write((char) c);

                        c = fr.read();
                    }
                    System.out.println(" ");
                } catch (Exception e) {

                    JOptionPane.showMessageDialog(null, e);

                }
                try {
                    fr.close();
                    fw.close();
                } catch (IOException e) {
                    JOptionPane.showMessageDialog(null, e);
                }

            }
        } catch (Exception e) {
            JOptionPane.showMessageDialog(null, e);
        }
    }}
