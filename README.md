/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package classwork;

/**
 *
 * @author atkins4440j
 */
public class RocketShip {
 public static void main(String[] args) {
        cone(6);
        firstLine();
        firstSquare(3);
    }
    public static void cone (int size) {
        for(int row = 1; row < size; row++){
            for(int col = 1; col < size - row; col++){
                System.out.print(" ");
            }
            for(int col = 0; col < row; col++){
                System.out.print("/");
            }
            System.out.print("**");
            for(int col = 0; col < row; col++){
                System.out.print("\\");
            }
            for(int col = 0; col < row; col++) {
                System.out.print("");
            }
            System.out.println();
        }
    }
    public static void firstLine(){
        System.out.println("+=*=*=*=*=*=*+");
    }
    public static void firstSquare(int dab) {
        for(int row = dab / 2; row >  0; row--){
                System.out.print("|");
            for(int col = 3; col > row; col--){
                System.out.print(".");
            }
            for(int col = 3; col > (dab / 2) - row; col--){
                System.out.print("\\/");
            }
            for(int col = 3; col > row; col--){
                System.out.print(".");
            }
            for(int col = 3; col > row; col--){
                System.out.print(".");
            }
            System.out.println();
        }
    }
}
