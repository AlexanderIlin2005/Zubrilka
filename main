# -*- coding: utf-8 -*-
import sys
import sqlite3
from PyQt5 import QtCore, QtWidgets
from PyQt5.QtCore import Qt
from PyQt5.QtGui import QPixmap
from PyQt5.QtPrintSupport import QPrintDialog, QPrinter
from PyQt5.QtWidgets import QApplication, QMainWindow, QFontDialog, QInputDialog, QMessageBox, QFileDialog


class Ui_Form(object):
    """Класс, где инициализируется графический пользовательский интерфейс программы"""

    def setup_ui(self, Form):
        Form.setObjectName("Form")
        Form.setGeometry(300, 300, 971, 693)
        self.text_zone = QtWidgets.QPlainTextEdit(Form)
        self.text_zone.setGeometry(QtCore.QRect(220, 20, 531, 621))
        self.text_zone.setObjectName("text_zone")
        self.about_btn = QtWidgets.QPushButton(Form)
        self.about_btn.setGeometry(QtCore.QRect(40, 230, 161, 32))
        self.about_btn.setObjectName("about_btn")
        self.font_btn = QtWidgets.QPushButton(Form)
        self.font_btn.setGeometry(QtCore.QRect(770, 130, 161, 31))
        self.font_btn.setObjectName("font_btn")
        self.cancel_btn = QtWidgets.QPushButton(Form)
        self.cancel_btn.setGeometry(QtCore.QRect(640, 650, 111, 32))
        self.cancel_btn.setObjectName("cancel_btn")
        self.next_btn = QtWidgets.QPushButton(Form)
        self.next_btn.setGeometry(QtCore.QRect(220, 650, 111, 32))
        self.next_btn.setObjectName("next_btn")
        self.open_file_btn = QtWidgets.QPushButton(Form)
        self.open_file_btn.setGeometry(QtCore.QRect(40, 40, 161, 31))
        self.open_file_btn.setObjectName("open_file_btn")
        self.horizontalSlider = QtWidgets.QSlider(Form)
        self.horizontalSlider.setGeometry(QtCore.QRect(360, 650, 231, 22))
        self.horizontalSlider.setOrientation(QtCore.Qt.Horizontal)
        self.horizontalSlider.setObjectName("horizontalSlider")
        self.difficulty_level = QtWidgets.QButtonGroup(Form)
        self.difficulty_level.setObjectName("difficulty_level")
        self.group = QtWidgets.QGroupBox(Form)
        self.group.setGeometry(QtCore.QRect(770, 240, 191, 301))
        self.group.setObjectName("group")
        self.radioButton = QtWidgets.QRadioButton(self.group)
        self.radioButton.setGeometry(QtCore.QRect(10, 30, 171, 20))
        self.radioButton.setObjectName("radioButton")
        self.difficulty_level.addButton(self.radioButton)
        self.radioButton_2 = QtWidgets.QRadioButton(self.group)
        self.radioButton_2.setGeometry(QtCore.QRect(10, 60, 171, 20))
        self.radioButton_2.setObjectName("radioButton_2")
        self.difficulty_level.addButton(self.radioButton_2)
        self.radioButton_3 = QtWidgets.QRadioButton(self.group)
        self.radioButton_3.setGeometry(QtCore.QRect(10, 120, 171, 20))
        self.radioButton_3.setObjectName("radioButton_3")
        self.difficulty_level.addButton(self.radioButton_3)
        self.radioButton_4 = QtWidgets.QRadioButton(self.group)
        self.radioButton_4.setGeometry(QtCore.QRect(10, 90, 171, 20))
        self.radioButton_4.setObjectName("radioButton_4")
        self.difficulty_level.addButton(self.radioButton_4)
        self.init_btn = QtWidgets.QPushButton(Form)
        self.init_btn.setGeometry(QtCore.QRect(770, 100, 161, 31))
        self.init_btn.setObjectName("init_btn")
        self.redact_btn = QtWidgets.QPushButton(Form)
        self.redact_btn.setGeometry(QtCore.QRect(770, 70, 161, 31))
        self.redact_btn.setObjectName("redact_btn")
        self.paste_btn = QtWidgets.QPushButton(Form)
        self.paste_btn.setGeometry(QtCore.QRect(770, 40, 161, 31))
        self.paste_btn.setObjectName("paste_btn")
        self.label_2 = QtWidgets.QLabel(Form)
        self.label_2.setGeometry(QtCore.QRect(50, 20, 141, 16))
        self.label_2.setObjectName("label_2")
        self.label_3 = QtWidgets.QLabel(Form)
        self.label_3.setGeometry(QtCore.QRect(50, 150, 141, 16))
        self.label_3.setObjectName("label_3")
        self.library_btn = QtWidgets.QPushButton(Form)
        self.library_btn.setGeometry(QtCore.QRect(40, 170, 161, 32))
        self.library_btn.setObjectName("library_btn")
        self.learn_btn = QtWidgets.QPushButton(Form)
        self.learn_btn.setGeometry(QtCore.QRect(40, 200, 161, 32))
        self.learn_btn.setObjectName("learn_btn")
        self.label_4 = QtWidgets.QLabel(Form)
        self.label_4.setGeometry(QtCore.QRect(780, 20, 141, 16))
        self.label_4.setObjectName("label_4")
        self.print_btn = QtWidgets.QPushButton(Form)
        self.print_btn.setGeometry(QtCore.QRect(40, 70, 161, 31))
        self.print_btn.setObjectName("print_btn")
        self.add_to_bd_btn = QtWidgets.QPushButton(Form)
        self.add_to_bd_btn.setGeometry(QtCore.QRect(40, 100, 161, 31))
        self.add_to_bd_btn.setObjectName("print_btn")
        self.label_5 = QtWidgets.QLabel(Form)
        self.label_5.setGeometry(QtCore.QRect(870, 670, 141, 16))
        self.label_5.setObjectName("label_5")
        self.icon_label = QtWidgets.QLabel(Form)
        self.icon_label.setGeometry(QtCore.QRect(0, 370, 220, 320))
        self.icon_label.setObjectName("icon_label")
        self.retranslate_ui(Form)
        QtCore.QMetaObject.connectSlotsByName(Form)

    def retranslate_ui(self, Form):
        _translate = QtCore.QCoreApplication.translate
        Form.setWindowTitle(_translate("Form", "Зубрилка"))
        self.text_zone.setPlainText(_translate("Form", "Вставьте сюда текст стихотворения "))
        self.about_btn.setText(_translate("Form", "О программе"))
        self.font_btn.setText(_translate("Form", "Выбрать шрифт"))
        self.cancel_btn.setText(_translate("Form", ">"))
        self.next_btn.setText(_translate("Form", "<"))
        self.open_file_btn.setText(_translate("Form", "Открыть файл"))
        self.add_to_bd_btn.setText(_translate("Form", "Добавить в каталог"))
        self.group.setTitle(_translate("Form", "Фильтры"))
        self.radioButton.setText(_translate("Form", "Показать первые буквы"))
        self.radioButton_2.setText(_translate("Form", "Скрыть слова"))
        self.radioButton_3.setText(_translate("Form", "Показать весь текст"))
        self.radioButton_4.setText(_translate("Form", "Скрыть весь текст"))
        self.init_btn.setText(_translate("Form", "Сохранить текст"))
        self.redact_btn.setText(_translate("Form", "Править текст"))
        self.paste_btn.setText(_translate("Form", "Вставить текст"))
        self.label_2.setText(_translate("Form", "Работа с файлом"))
        self.label_3.setText(_translate("Form", "Полезные материалы"))
        self.library_btn.setText(_translate("Form", "Библиотека"))
        self.learn_btn.setText(_translate("Form", "О методике"))
        self.label_4.setText(_translate("Form", "Работа с текстом"))
        self.print_btn.setText(_translate("Form", "Напечатать"))
        self.label_5.setToolTip(_translate("Form", "<html><head/><body><p>Ильин А., 2020</p></body></html>"))
        self.label_5.setText(_translate("Form", "Ильин А. 2020"))


class App_Main_Window(QMainWindow, Ui_Form):
    def __init__(self):
        super().__init__()
        self.pixmap = QPixmap('pen.png')
        self.setWindowFlags(Qt.CustomizeWindowHint | Qt.WindowCloseButtonHint | Qt.WindowMinimizeButtonHint)
        self.text_zone_list = []
        self.setup_ui(self)
        self.stadia = 0
        self.text_redacted = True
        self.cancel_btn.setEnabled(False)
        self.next_btn.setEnabled(False)
        self.redact_btn.setEnabled(False)
        self.paste_btn.setEnabled(True)
        self.open_file_btn.setEnabled(True)
        self.group.setEnabled(False)
        self.horizontalSlider.setEnabled(False)
        self.horizontalSlider.setValue(4)
        self.horizontalSlider.setMinimum(0)
        self.horizontalSlider.setMaximum(4)
        self.radioButton.setChecked(True)
        self.add_to_bd_btn.setEnabled(False)
        self.function_connects()

    def function_connects(self):
        """Функция, подключающая обработчики событий к виджетам"""
        self.try_open_file()
        self.init_btn.clicked.connect(self.start)
        self.font_btn.clicked.connect(self.set_font)
        self.about_btn.clicked.connect(self.show_info)
        self.cancel_btn.clicked.connect(self.degrade_stadia)
        self.next_btn.clicked.connect(self.ubgrade_stadia)
        self.redact_btn.clicked.connect(self.redact_text)
        self.paste_btn.clicked.connect(self.paste)
        self.open_file_btn.clicked.connect(self.open_file)
        self.difficulty_level.buttonClicked.connect(self.main_process)
        self.horizontalSlider.valueChanged.connect(self.set_stadia_by_slider)
        self.print_btn.clicked.connect(self.printer)
        self.learn_btn.clicked.connect(self.how_to_learn)
        self.set_icon()
        self.library_btn.clicked.connect(self.open_library_window)
        self.add_to_bd_btn.clicked.connect(self.add_to_bd)

    def add_to_bd(self):
        con = sqlite3.connect("poema_db.db")
        cur = con.cursor()
        name, ok_pressed = QInputDialog.getText(self, "Добавление в библиотеку",
                                                "Укажите имя автора и название стихотворения")
        if ok_pressed:
            path = f"Стихи/{name}.txt"
            with open(path, "w") as f:
                for line in self.text_zone_list:
                    f.write(line + "\n")
            update = f"""INSERT INTO poems(Author, path) VALUES("{name}", "{path}")"""
            cur.execute(update)
            con.commit()
        con.close()

    def open_library_window(self):
        """Функция, отвечающая за работу с БД"""
        list_for_dialog = []
        con = sqlite3.connect("poema_db.db")
        cur = con.cursor()
        get1 = """SELECT Author FROM poems"""
        result1 = cur.execute(get1).fetchall()
        for elem in result1:
            list_for_dialog.append(elem[0])
        author, ok_pressed = QInputDialog.getItem(
            self, "Библиотека", "Выберите автора",
            tuple(list_for_dialog), 1, False)
        if ok_pressed:
            get2 = f'SELECT path FROM poems WHERE Author = "{author}"'
            result2 = cur.execute(get2).fetchone()

            # Вывод результатов на экран
            path = result2[0]

            con.close()
            self.open_chosen_file(path_=path)

    def open_chosen_file(self, path_):
        """Функция открывает выбранный пользователем стих"""
        with open(path_, "r") as f:
            self.text_zone.clear()
            self.text_zone_list.clear()
            for line in f.readlines():
                line2 = "".join([sym for sym in line if sym != "\n"])
                # self.text_zone_list.append(line)
                self.text_zone_list.append(line2)

            for line1 in self.text_zone_list:
                self.text_zone.appendPlainText(line1)

    def set_icon(self):
        """Настройка иконки приложения"""
        self.pixmap.scaled(220, 320)
        self.icon_label.setPixmap(self.pixmap)
        self.repaint()

    def how_to_learn(self):
        """Показывает пользователю методику выучивания стихотворений"""
        msg_text = """
1. Загрузите текст стихотворения в «Зубрилку».
2. Сохраните его, нажав кнопку «Сохранить»
3. Выберите шрифт, размер текста. 
4. Прочитайте текст вслух несколько раз.
5. Определите структуру текста. 
6. Выделите запоминающиеся слова. 
7. Уточните смысл непонятных слов. 
8. Прочитайте стихотворение с выражением.
9. Начните учить, повышая уровень сложности.
10. Учите, опираясь на первые буквы в строках. 
11. Расскажите стихотворение наизусть!
        """
        msg = QMessageBox(self)
        msg.setIcon(QMessageBox.Information)
        msg.setText("Рекомендации по заучиванию стихотворений:")
        msg.setInformativeText(msg_text)
        msg.setStandardButtons(QMessageBox.Ok)
        msg.button(QMessageBox.Ok).setText("Прочитано")
        msg.show()

    def printer(self):
        """Печать текста на принтер"""
        printer = QPrinter(QPrinter.HighResolution)
        dialog = QPrintDialog(printer, self)
        if dialog.exec_() == QPrintDialog.Accepted:
            self.text_zone.print_(printer)

    def set_stadia_by_slider(self):
        """изменение сложности при изменении значения слайдера"""
        lst = {4: 0, 3: 1, 2: 2, 1: 3, 0: 4}
        self.stadia = lst[self.horizontalSlider.value()]
        if self.radioButton.isChecked():
            self.simple_version_process()
        elif self.radioButton_2.isChecked():
            self.difficult_version_process()
        self.repaint()

    def try_open_file(self):
        """Открывает сохраненный файл"""
        try:
            with open("poem.txt", "r") as f:
                self.text_zone.clear()
                self.text_zone_list.clear()
                for line in f.readlines():
                    line2 = "".join([sym for sym in line if sym != "\n"])
                    # self.text_zone_list.append(line)
                    self.text_zone_list.append(line2)

                for line1 in self.text_zone_list:
                    self.text_zone.appendPlainText(line1)
        except FileNotFoundError:
            self.text_zone.setPlainText("Удалите эту строку и вставьте сюда текст стихотворения без названия")

    def paste(self):
        """Вставляет текст из буфера обмена (CTRL/CMD + V)"""
        text = QApplication.clipboard().text()
        self.text_zone.clear()
        self.text_zone.setPlainText(text)
        self.text_zone.repaint()

    def open_file(self):
        """Открытие выбранного пользователем файла"""
        fname = QFileDialog.getOpenFileName(self, 'Open file', '', "Text files (*.txt)")[0]
        if fname != "":
            with open(fname, 'r') as f:
                self.text_zone_list.clear()
                self.text_zone.clear()
                for line in f.readlines():
                    self.text_zone_list.append(line)
                    self.text_zone.appendPlainText(line)

    def set_font(self):
        """Настройка шрифта текста"""
        font, ok = QFontDialog.getFont()
        if ok:
            self.text_zone.setFont(font)
        self.text_zone.repaint()

    def show_info(self):
        """Показывает описание функционала приложения"""
        msg_text = """
Программа для заучивания стихотворений «Зубрилка»
помогает быстро и эффективно запоминать
стихотворения. «Зубрилка» основана на методепоэтапного
закрытия слов в строке. Этот способ заучивания десятилетиями
успешно применяли школьники и студенты. Программа «Зубрилка»
помогает организовать процесс запоминания наиболее эффективно,
задействует зрительную память, структурирует процесс заучивания,
постепенно повышая сложность.

Функционал программы позволяет автоматически скрывать слова в 
строке по мере заучивания, оставлять первые буквы слов для подсказки.
Программа позволяет открыть документ с компьютера или загрузить текст,
редактировать его, сохранить стихотворение. В программе имеется справка,
советы по эффективному заучиванию, библиотека стихотворений. Программа 
будет полезна школьникам и студентам гуманитарных ВУЗов, а также всем
любителям поэзии.
        """
        msg = QMessageBox(self)
        msg.setIcon(QMessageBox.Information)
        msg.setText("О приложении")
        msg.setInformativeText(msg_text)
        msg.setStandardButtons(QMessageBox.Ok)
        msg.button(QMessageBox.Ok).setText("Прочитано")
        msg.show()

    def ubgrade_stadia(self):
        """Увеличение уровня сложности"""
        lst = {4: 0, 3: 1, 2: 2, 1: 3, 0: 4}
        if self.stadia < 4:
            self.stadia = self.stadia + 1
            self.horizontalSlider.setValue(lst[self.stadia])
            self.horizontalSlider.repaint()
        self.main_process()

    def degrade_stadia(self):
        """Уменьшение уровня сложности"""
        lst = {4: 0, 3: 1, 2: 2, 1: 3, 0: 4}
        if self.stadia > 0:
            self.stadia = self.stadia - 1
            self.horizontalSlider.setValue(lst[self.stadia])
            self.horizontalSlider.repaint()
        self.main_process()

    def closeEvent(self, event):
        """Функция отвечает за действия, происходящие при закрытии приложения"""
        reply = QMessageBox.question(
            self, "Message",
            "Сохранить стих перед закрытием",
            QMessageBox.Ok | QMessageBox.Cancel)

        if reply == QMessageBox.Ok:
            with open("poem.txt", "w") as f:
                for line in self.text_zone_list:
                    f.write(line + "\n")

            app.quit()
        else:
            app.quit()

    def main_process(self):
        """Главный алгоритм"""
        if self.radioButton.isChecked():
            self.simple_version_process()
        elif self.radioButton_2.isChecked():
            self.difficult_version_process()
        elif self.radioButton_3.isChecked():
            self.cancel_btn.setEnabled(False)
            self.next_btn.setEnabled(False)
            self.horizontalSlider.setEnabled(False)
            self.show_text()
        elif self.radioButton_4.isChecked():
            self.cancel_btn.setEnabled(False)
            self.next_btn.setEnabled(False)
            self.horizontalSlider.setEnabled(False)
            self.hide_text()

    def show_text(self):
        """Полный открытый показ текста"""
        self.text_zone.clear()
        for line in self.text_zone_list:
            self.text_zone.appendPlainText(line)

    def hide_text(self):
        """Полное скрытие текста"""
        self.text_zone.clear()
        for line in self.text_zone_list:
            self.text_zone.appendPlainText("*" * len(line))

    def start(self):
        """Коней редактированию текста"""
        self.add_to_bd_btn.setEnabled(True)
        self.library_btn.setEnabled(False)
        self.text_zone_list.clear()
        self.next_btn.setEnabled(True)
        self.cancel_btn.setEnabled(True)
        self.init_btn.setEnabled(False)
        self.redact_btn.setEnabled(True)
        self.text_zone.setReadOnly(True)
        self.paste_btn.setEnabled(False)
        self.open_file_btn.setEnabled(False)
        # self.difficulty_level.setEnabled(True)
        for line in self.text_zone.toPlainText().split("\n"):
            self.text_zone_list.append(line)
        self.group.setEnabled(True)
        self.horizontalSlider.setEnabled(True)
        self.repaint()

    def redact_text(self):
        """Переход в режим редактирования текста"""
        self.library_btn.setEnabled(True)
        self.add_to_bd_btn.setEnabled(False)
        self.text_zone.clear()
        for line in self.text_zone_list:
            self.text_zone.appendPlainText(line)
        self.next_btn.setEnabled(False)
        self.cancel_btn.setEnabled(False)
        self.init_btn.setEnabled(True)
        self.redact_btn.setEnabled(False)
        self.text_zone.setReadOnly(False)
        self.paste_btn.setEnabled(True)
        self.open_file_btn.setEnabled(True)
        self.group.setEnabled(False)
        self.horizontalSlider.setEnabled(False)
        self.repaint()

    def simple_version_process(self):
        self.next_btn.setEnabled(True)
        self.cancel_btn.setEnabled(True)
        self.horizontalSlider.setEnabled(True)
        insert_value = self.stadia
        self.text_zone.clear()
        if insert_value == 0:
            self.cancel_btn.setEnabled(False)
            self.show_text()
        elif insert_value in [1, 2]:
            self.text_zone.clear()
            self.next_btn.setEnabled(True)
            self.cancel_btn.setEnabled(True)
            for line in self.text_zone_list:
                formatted_line_list = []
                line_list_of_words = line.split()
                normal_words, stars_words = line_list_of_words[0:len(line_list_of_words) - insert_value], \
                                            line_list_of_words[(len(line_list_of_words) - insert_value)::]
                for word in normal_words:
                    formatted_line_list.append(word)
                for word in stars_words:
                    formatted_line_list.append(word[0] + ("*" * (len(word) - 1)))
                formatted_line = " ".join(formatted_line_list)
                self.text_zone.appendPlainText(formatted_line)
        elif insert_value == 3:
            self.text_zone.clear()
            self.next_btn.setEnabled(True)
            self.cancel_btn.setEnabled(True)
            for line in self.text_zone_list:
                formatted_line_list = []
                line_list_of_words = line.split()
                normal_words, stars_words = line_list_of_words[0:1], \
                                            line_list_of_words[1::]
                for word in normal_words:
                    formatted_line_list.append(word)
                for word in stars_words:
                    formatted_line_list.append(word[0] + ("*" * (len(word) - 1)))
                formatted_line = " ".join(formatted_line_list)
                self.text_zone.appendPlainText(formatted_line)
        elif insert_value == 4:
            self.text_zone.clear()
            self.next_btn.setEnabled(False)
            for line in self.text_zone_list:
                formatted_line_list = []
                line_list_of_words = line.split()
                stars_words = line_list_of_words[::]
                for word in stars_words:
                    formatted_line_list.append(word[0] + ("*" * (len(word) - 1)))
                formatted_line = " ".join(formatted_line_list)
                self.text_zone.appendPlainText(formatted_line)
        self.repaint()

    def difficult_version_process(self):
        self.next_btn.setEnabled(True)
        self.cancel_btn.setEnabled(True)
        self.horizontalSlider.setEnabled(True)
        self.text_zone.clear()
        insert_value = self.stadia
        if insert_value == 0:
            self.cancel_btn.setEnabled(False)
            self.show_text()
        elif insert_value in [1, 2]:
            self.text_zone.clear()
            self.next_btn.setEnabled(True)
            self.cancel_btn.setEnabled(True)
            for line in self.text_zone_list:
                formatted_line_list = []
                line_list_of_words = line.split()
                normal_words, stars_words = line_list_of_words[0:len(line_list_of_words) - insert_value], \
                                            line_list_of_words[(len(line_list_of_words) - insert_value)::]
                for word in normal_words:
                    formatted_line_list.append(word)
                for word in stars_words:
                    formatted_line_list.append("*" * len(word))
                formatted_line = " ".join(formatted_line_list)
                self.text_zone.appendPlainText(formatted_line)
        elif insert_value == 3:
            self.text_zone.clear()
            self.next_btn.setEnabled(True)
            self.cancel_btn.setEnabled(True)
            for line in self.text_zone_list:
                formatted_line_list = []
                line_list_of_words = line.split()
                normal_words, stars_words = line_list_of_words[0:1], \
                                            line_list_of_words[1::]
                for word in normal_words:
                    formatted_line_list.append(word)
                for word in stars_words:
                    formatted_line_list.append("*" * len(word))
                formatted_line = " ".join(formatted_line_list)
                self.text_zone.appendPlainText(formatted_line)
        elif insert_value == 4:
            self.text_zone.clear()
            self.next_btn.setEnabled(False)
            for line in self.text_zone_list:
                formatted_line_list = []
                line_list_of_words = line.split()
                stars_words = line_list_of_words[::]
                for word in stars_words:
                    formatted_line_list.append("*" * len(word))
                formatted_line = " ".join(formatted_line_list)
                self.text_zone.appendPlainText(formatted_line)
        self.repaint()


if __name__ == '__main__':
    app = QApplication(sys.argv)
    ex = App_Main_Window()
    ex.show()
    sys.exit(app.exec_())
