# HYBJ
import java.awt.Color;

import javax.swing.*;

public class HYBJ {

	private JFrame frame;

	// Table (테이블판)

	private JPanel table_panel;
	private JLabel Table_1;
	private JLabel Table_2;
	private JLabel Table_3;
	private JLabel Table_4;
	private JLabel Table_5;
	private JLabel Table_6;
	private JLabel Table_7;
	private JLabel Table_8;
	private JLabel Table_9;
	private JLabel Table_10;

	// Menu (메뉴판)

	private JPanel Menu_panel;
	private JButton Menu_1;
	private JButton Menu_2;
	private JButton Menu_3;
	private JButton Menu_4;
	private JButton Menu_5;

	// order(주문현황판)

	private JPanel order_panel;
	private JButton orderAdd;
	private JButton orderCancel;
	private JButton orderChange;
	private JButton orderCheck;
	private JTextArea ShowOrder;
	private JComboBox table_num;
	private String[] table_num_array = { "1", "2", "3", "4", "5", "6", "7",
			"8", "9", "10" };

	// Find (검색 판)
	private JPanel Find_panel;
	private JButton FindName;
	private JButton FindMoney;
	private JTextArea ShowResult;
	private JTextField inputName;
	private JTextField inputMoney;

	//
	public void makeTablePanel() {
		table_panel = new JPanel();
		table_panel.setLayout(null);
		table_panel.setBounds(50, 80, 290, 155);
		table_panel.setBorder(BorderFactory.createEtchedBorder());

		JLabel panel_name = new JLabel("=====좌석현황=====");
		panel_name.setBounds(50, 60, 190, 15);
		frame.add(panel_name);

		Table_1 = new JLabel("1");
		Table_1.setOpaque(true);
		Table_1.setBounds(10, 20, 50, 50);
		Table_1.setBorder(BorderFactory.createEtchedBorder());
		Table_1.setBackground(Color.white);
		Table_1.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_1);

		Table_2 = new JLabel("2");
		Table_2.setOpaque(true);
		Table_2.setBounds(65, 20, 50, 50);
		Table_2.setBorder(BorderFactory.createEtchedBorder());
		Table_2.setBackground(Color.white);
		Table_2.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_2);

		Table_3 = new JLabel("3");
		Table_3.setOpaque(true);
		Table_3.setBounds(120, 20, 50, 50);
		Table_3.setBorder(BorderFactory.createEtchedBorder());
		Table_3.setBackground(Color.white);
		Table_3.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_3);

		Table_4 = new JLabel("4");
		Table_4.setOpaque(true);
		Table_4.setBounds(175, 20, 50, 50);
		Table_4.setBorder(BorderFactory.createEtchedBorder());
		Table_4.setBackground(Color.white);
		Table_4.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_4);

		Table_5 = new JLabel("5");
		Table_5.setOpaque(true);
		Table_5.setBounds(230, 20, 50, 50);
		Table_5.setBorder(BorderFactory.createEtchedBorder());
		Table_5.setBackground(Color.white);
		Table_5.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_5);

		Table_6 = new JLabel("6");
		Table_6.setOpaque(true);
		Table_6.setBounds(10, 85, 50, 50);
		Table_6.setBorder(BorderFactory.createEtchedBorder());
		Table_6.setBackground(Color.white);
		Table_6.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_6);

		Table_7 = new JLabel("7");
		Table_7.setOpaque(true);
		Table_7.setBounds(65, 85, 50, 50);
		Table_7.setBorder(BorderFactory.createEtchedBorder());
		Table_7.setBackground(Color.white);
		Table_7.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_7);

		Table_8 = new JLabel("8");
		Table_8.setOpaque(true);
		Table_8.setBounds(120, 85, 50, 50);
		Table_8.setBorder(BorderFactory.createEtchedBorder());
		Table_8.setBackground(Color.white);
		Table_8.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_8);

		Table_9 = new JLabel("9");
		Table_9.setOpaque(true);
		Table_9.setBounds(175, 85, 50, 50);
		Table_9.setBorder(BorderFactory.createEtchedBorder());
		Table_9.setBackground(Color.white);
		Table_9.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_9);

		Table_10 = new JLabel("10");
		Table_10.setOpaque(true);
		Table_10.setBounds(230, 85, 50, 50);
		Table_10.setBorder(BorderFactory.createEtchedBorder());
		Table_10.setBackground(Color.white);
		Table_10.setHorizontalAlignment(SwingConstants.CENTER);
		table_panel.add(Table_10);
	}

	public void makeOrderPanel() {
		order_panel = new JPanel();
		order_panel.setLayout(null);
		order_panel.setBounds(400, 80, 300, 240);
		order_panel.setBorder(BorderFactory.createEtchedBorder());

		JLabel panel_name = new JLabel("=========주문현황=========");
		panel_name.setBounds(400, 60, 190, 15);
		frame.add(panel_name);

		ShowOrder = new JTextArea();
		ShowOrder.setOpaque(true);
		ShowOrder.setBounds(15, 15, 180, 210);
		ShowOrder.setBorder(BorderFactory.createEtchedBorder());
		order_panel.add(ShowOrder);

		orderAdd = new JButton("추가");
		orderAdd.setOpaque(true);
		orderAdd.setBounds(210, 15, 60, 30);
		orderAdd.setBorder(BorderFactory.createEtchedBorder());
		order_panel.add(orderAdd);

		orderCancel = new JButton("취소");
		orderCancel.setOpaque(true);
		orderCancel.setBounds(210, 55, 60, 30);
		orderCancel.setBorder(BorderFactory.createEtchedBorder());
		order_panel.add(orderCancel);

		orderChange = new JButton("수정");
		orderChange.setOpaque(true);
		orderChange.setBounds(210, 95, 60, 30);
		orderChange.setBorder(BorderFactory.createEtchedBorder());
		order_panel.add(orderChange);

		orderCheck = new JButton("결제");
		orderCheck.setOpaque(true);
		orderCheck.setBounds(210, 135, 60, 30);
		orderCheck.setBorder(BorderFactory.createEtchedBorder());
		order_panel.add(orderCheck);

		table_num = new JComboBox();
		table_num.setModel(new DefaultComboBoxModel(table_num_array));
		table_num.setBounds(210, 175, 60, 30);
		table_num.setBorder(BorderFactory.createEtchedBorder());
		order_panel.add(table_num);

	}

	public void makeMenupanPanel() {
		Menu_panel = new JPanel();
		Menu_panel.setLayout(null);
		Menu_panel.setBounds(50, 400, 300, 110);
		Menu_panel.setBorder(BorderFactory.createEtchedBorder());

		JLabel panel_name = new JLabel("***** 메뉴판 *****");
		panel_name.setBounds(50, 380, 190, 15);
		frame.add(panel_name);

		Menu_1 = new JButton("짜장면");
		Menu_1.setOpaque(true);
		Menu_1.setBounds(20, 10, 100, 25);
		Menu_1.setBorder(BorderFactory.createEtchedBorder());
		Menu_panel.add(Menu_1);

		Menu_2 = new JButton("짬뽕");
		Menu_2.setOpaque(true);
		Menu_2.setBounds(20, 40, 100, 25);
		Menu_2.setBorder(BorderFactory.createEtchedBorder());
		Menu_panel.add(Menu_2);

		Menu_3 = new JButton("볶음밥");
		Menu_3.setOpaque(true);
		Menu_3.setBounds(20, 70, 100, 25);
		Menu_3.setBorder(BorderFactory.createEtchedBorder());
		Menu_panel.add(Menu_3);

		Menu_4 = new JButton("군만두");
		Menu_4.setOpaque(true);
		Menu_4.setBounds(160, 20, 100, 30);
		Menu_4.setBorder(BorderFactory.createEtchedBorder());
		Menu_panel.add(Menu_4);

		Menu_5 = new JButton("음료수");
		Menu_5.setOpaque(true);
		Menu_5.setBounds(160, 60, 100, 30);
		Menu_5.setBorder(BorderFactory.createEtchedBorder());
		Menu_panel.add(Menu_5);

	}

	public void makeFindPanel() {
		Find_panel = new JPanel();
		Find_panel.setLayout(null);
		Find_panel.setBounds(400, 400, 300, 200);
		Find_panel.setBorder(BorderFactory.createEtchedBorder());
		
		JLabel panel_name = new JLabel("★★★★ 조회(고객찾기) ★★★★");
		panel_name.setBounds(400, 280, 300, 200);
		frame.add(panel_name);
		
		FindName = new JButton("이름으로찾기");
		FindName.setOpaque(true);
		FindName.setBounds(20, 40 , 110, 30);
		FindName.setBorder(BorderFactory.createEtchedBorder());
		Find_panel.add(FindName);
		
		FindMoney = new JButton("금액으로찾기");
		FindMoney.setOpaque(true);
		FindMoney.setBounds(160, 40 , 110, 30);
		FindMoney.setBorder(BorderFactory.createEtchedBorder());
		Find_panel.add(FindMoney);
		
		inputName = new JTextField();
		inputName.setOpaque(true);
		inputName.setBounds(20, 10, 110, 25);
		Find_panel.add(inputName);
		
		inputMoney= new JTextField();
		inputMoney.setOpaque(true);
		inputMoney.setBounds(160, 10, 110, 25);
		Find_panel.add(inputMoney);
		
		ShowResult= new JTextArea();
		ShowResult.setOpaque(true);
		ShowResult.setBounds(20, 80 ,250,100);
		ShowResult
		.setBorder(BorderFactory.createEtchedBorder());
		Find_panel.add(ShowResult);

	}

	public HYBJ() {
		frame = new JFrame("한양반점");
		frame.setLayout(null);
		frame.setBounds(200, 100, 700, 700);

		makeTablePanel();
		frame.add(table_panel);

		makeOrderPanel();
		frame.add(order_panel);

		makeMenupanPanel();
		frame.add(Menu_panel);
		
		makeFindPanel();
		frame.add(Find_panel);

		frame.setTitle(" <<<< 한양반점 >>>>");
		frame.setSize(750, 680);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.setVisible(true);
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		new HYBJ();

	}

}
