# TugasAlgoritmaPemrograman
# Bangun Ruang

        import java.util.Scanner;

        public class HitungBangunRuang {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int pilihan;

        do {
            System.out.println("\n--- Program Hitung Volume Bangun Ruang ---");
            System.out.println("1. Kubus");
            System.out.println("2. Balok");
            System.out.println("3. Tabung");
            System.out.println("4. Keluar");
            System.out.print("Pilih bangun ruang (1-4): ");
            pilihan = scanner.nextInt();

            switch (pilihan) {
                case 1:
                    System.out.print("Masukkan sisi kubus: ");
                    double sisi = scanner.nextDouble();
                    double volKubus = sisi * sisi * sisi;
                    System.out.println("Volume Kubus: " + volKubus);
                    break;
                case 2:
                    System.out.print("Masukkan panjang balok: ");
                    double p = scanner.nextDouble();
                    System.out.print("Masukkan lebar balok: ");
                    double l = scanner.nextDouble();
                    System.out.print("Masukkan tinggi balok: ");
                    double t = scanner.nextDouble();
                    double volBalok = p * l * t;
                    System.out.println("Volume Balok: " + volBalok);
                    break;
                case 3:
                    System.out.print("Masukkan jari-jari tabung: ");
                    double r = scanner.nextDouble();
                    System.out.print("Masukkan tinggi tabung: ");
                    double tTabung = scanner.nextDouble();
                    double volTabung = Math.PI * r * r * tTabung;
                    System.out.println("Volume Tabung: " + volTabung);
                    break;
                case 4:
                    System.out.println("Keluar dari program.");
                    break;
                default:
                    System.out.println("Pilihan tidak valid.");
            }
        } while (pilihan != 4);

        scanner.close();
    }
 }

