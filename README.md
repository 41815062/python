{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyPDyJRpewJRf8W1w6+KUhay",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/41815062/python/blob/main/README.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "id": "N3rtPnSlhj34"
      },
      "outputs": [],
      "source": []
    },
    {
      "cell_type": "markdown",
      "source": [],
      "metadata": {
        "id": "WTHXCTaqhq6Z"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "#CH1. 파이썬 문법\n",
        "## 자료형\n",
        "**숫자형**  \n",
        "  \n",
        "* 정수 : 123, 456, 0. -30  \n",
        "* 실수 : 12.345. -987,65 0.7e6  \n",
        "* 8진수 : 0o765, 0o123\n",
        "* 16진수 : 0x0D, 0x0A, 0xFF  \n",
        "\n",
        "**변수**  \n",
        "* 문자 또는 밑줄로 시작(_kim, alpha)  \n",
        "* 대소문자 구분(sum, Sum, SUM)  \n",
        "* 영문자, 숫자, 밑줄(A~z, 0-9, _)  \n",
        " ex) sun_9, Alpha, s9n)  \n",
        "* 파이썬 키워드(print...)  \n",
        "\n",
        "**표기법**  \n",
        "+ 카멜(낙타) : myNAME  \n",
        "+ 스네이크(뱀) : my_name  \n",
        "+ 파스칼 : MyName\n",
        "\n",
        "\n"
      ],
      "metadata": {
        "id": "lYZB82C_htyh"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "a = 10\n",
        "b = 20 \n",
        "f = \"10\"\n",
        "c = a+b\n",
        "print(a,b,c,f)\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "nkToiLJFlXcr",
        "outputId": "3a263105-d171-43aa-c4b4-f4aff399a5b3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "10 20 30 10\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = 10\n",
        "b = 20\n",
        "c = \"10\"\n",
        "d = \"20\"\n",
        "\n",
        "print(a+b)\n",
        "print(a,b)\n",
        "print(type(a))\n",
        "print(type(b))\n",
        "print (a+b)\n",
        "print(c+d)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "jmZgkwy7l-Ea",
        "outputId": "eaf6735d-d152-4bd2-ca75-1308e05bf8e9"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "30\n",
            "10 20\n",
            "<class 'int'>\n",
            "<class 'int'>\n",
            "30\n",
            "1020\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# 나눗셈\n",
        "a = 10\n",
        "b = 3\n",
        "c = a / b\n",
        "d = a // b # 몫\n",
        "e = a % b # 나머지 ex(홀짝 LED 깜빡임)\n",
        "print(c,d,e)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "jd9yqIUPqYjr",
        "outputId": "ee11cbc0-f0c9-494c-9937-76007603cde8"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "3.3333333333333335 3 1\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# 곱셈\n",
        "a = 10\n",
        "b = 3\n",
        "c = a * b # 곱하기\n",
        "d = a**b # 제곱\n",
        "print(c, d)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "9s2oZbiErHWE",
        "outputId": "6a184107-a7ab-4cc1-f7dd-e1b893e7eace"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "30 1000\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### 문자열\n",
        "1. 큰따옴표 : \"Woo Jin\"\n",
        "2. 작은따옴표 : 'Woo Jin'\n",
        "3. 큰 따옴표 3개 : \"\"\"대한민국\"\"\"\n",
        "4. 작은 따옴표 3개 : '''대한민국'''\n",
        "5. \"동해물과 백두산이 마르고 닳도록 kim's\\\""
      ],
      "metadata": {
        "id": "p5v0SkMlrjjr"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# 변수\n",
        "myName = \"Lee Woo Jin\"\n",
        "my_name = '이우진'\n",
        "_my_name = \"korea\"\n",
        "MYNAME = \"코리아\"\n",
        "my2name = \"kikiki\"\n",
        "# 2myname = \"숫자먼저\"\n",
        "# 시험 실수 하는 것 my-name = \"마이너스\"\n",
        "# my name = \"스페이스\"\n",
        "myName1 = 1234\n",
        "myName2 = \"1234\"\n",
        "print(type(myName1))\n",
        "print(type(myName2))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "E5clc72qtbRt",
        "outputId": "7cbd4fd3-947c-4860-a9d1-357da861316c"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "<class 'int'>\n",
            "<class 'str'>\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### 변수할당"
      ],
      "metadata": {
        "id": "yJVTPbLcuuoc"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "a=b=c= \"브라보콘\"\n",
        "print(a)\n",
        "print(b)\n",
        "print(c)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "H0Yx6Kw0uzP8",
        "outputId": "4cf5853b-82c6-4931-e302-f6315c95d32d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "브라보콘\n",
            "브라보콘\n",
            "브라보콘\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "x,y,z = \"딸기\", \"포도\" , \"바나나\"\n",
        "print(x,y,z)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "KlGSO8_4vMXa",
        "outputId": "9e9b93d6-3365-428c-a7fc-890982fe811e"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "딸기 포도 바나나\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "fruits=[\"누가바\",\"쌍쌍바\", \"보석바\"]\n",
        "x,y,z = fruits \n",
        "print(x)\n",
        "print(y)\n",
        "print(z)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "9suPxDjTv6cl",
        "outputId": "55f96a11-f0be-48c0-f21c-0166d6e43a24"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "누가바\n",
            "쌍쌍바\n",
            "보석바\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "x = \"Life\"\n",
        "y = \"is\"\n",
        "z = \"beatiful!\"\n",
        "print(x,y,z)\n",
        "print(x+y+z)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "HPozvHskwgjF",
        "outputId": "ca2fa9b6-b913-447a-9903-d9778c22e5c1"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Life is beatiful!\n",
            "Lifeisbeatiful!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = 1\n",
        "b = 2\n",
        "c = 3\n",
        "print(a+b+c)\n",
        "print(a,b,c)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "X47s32WuxMWN",
        "outputId": "8ea32ac0-9d4c-4090-f377-a3b1edd30f64"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "6\n",
            "1 2 3\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = '1'\n",
        "b = '2'\n",
        "c = '3'\n",
        "print(a+b+c)\n",
        "print(a,b,c)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "lL_-BVwAxZHf",
        "outputId": "d8f7227c-4d48-4270-c59b-8165174d67f5"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "123\n",
            "1 2 3\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "데이터 바꾸기"
      ],
      "metadata": {
        "id": "S5iPU8_z758o"
      }
    },
    {
      "cell_type": "code",
      "source": [
        " a = 1; b = 2\n",
        " a, b = b , a\n",
        "print(a,b)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "jOT73j3k78t4",
        "outputId": "f514514a-58e8-4e05-80b2-055d36a5b569"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "2 1\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "b = 2; c = 3\n",
        "#c = (b=b+c) //에러발생"
      ],
      "metadata": {
        "id": "xwzk83EO8Sho"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "a=1;b=1;c=3\n",
        "f = a + b + \\  # \\ 줄바꿈\n",
        "c\n",
        "print(f)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "tw0o9VVz8lH4",
        "outputId": "46445dad-4958-4c2b-d866-16ed9bb80ecd"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "5\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# len()\n",
        "\n",
        "a = '123456'\n",
        "b = [2,3,4,5]   # 숫자는 배열로 잡아줘야 길이나타내기 가능\n",
        "print(len(a))\n",
        "print(len(b))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "eCx_Yr6R86Uo",
        "outputId": "fa6db838-5df4-4682-8a65-9c8caf7cd683"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "6\n",
            "4\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#### 계산기"
      ],
      "metadata": {
        "id": "kRQKNWl39YCo"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "a = 100\n",
        "b = 200\n",
        "result=a+b\n",
        "print(a,'+',b,'=',result)\n",
        "result = a - b\n",
        "print(a,'-',b,'=',result)\n",
        "result=a/b\n",
        "print(a,'/',b,'=',result)\n",
        "result = a * b\n",
        "print(a,'*',b,'=',result)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "W2xw6ijf9a8B",
        "outputId": "a70c654d-2880-4f24-cc47-bfb181baee4b"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "100 + 200 = 300\n",
            "100 - 200 = -100\n",
            "100 / 200 = 0.5\n",
            "100 * 200 = 20000\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = \"1234\"\n",
        "b = 5678\n",
        "c = int(a)+ b # 형 변환\n",
        "print(c)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "1SD3r2gIAp1K",
        "outputId": "d20c3e5a-c0ac-4148-8cba-eb53cf57f9ce"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "6912\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# 계산기 2\n",
        "num1 = int(input(\"숫자입력1:  \"))\n",
        "num2 = int(input(\"숫자입력2:  \"))\n",
        "print(type(num1))\n",
        "\n",
        "result1 = num1 + num2\n",
        "result2 = num1 - num2\n",
        "result3 = num1 * num2\n",
        "result4 = num1 / num2\n",
        "print(result1,result2,result3,result4)\n",
        "result=num1+num2\n",
        "print(num1,'+',num2,'=',result)\n",
        "result =num1-num2\n",
        "print(num1,'-',num2,'=',result)\n",
        "result=num1/num2\n",
        "print(num1,'/',num2,'=',result)\n",
        "result = num1 * num2\n",
        "print(num1,'*',num2,'=',result)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "W0WqFUZsBAQR",
        "outputId": "e04cc586-4380-4f52-d366-b1404dd5fbf3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "숫자입력1:  10\n",
            "숫자입력2:  5\n",
            "<class 'int'>\n",
            "15 5 50 2.0\n",
            "10 + 5 = 15\n",
            "10 - 5 = 5\n",
            "10 / 5 = 2.0\n",
            "10 * 5 = 50\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "# 자기이름, 전화번호, 택배(g)*100\n",
        "# 결과값 = g * 100원 = 00원입니다.\n",
        "a = input(\"이름입력:  \")\n",
        "b = input(\"전화번호입력:  \")\n",
        "c = int(input(\"택배g입력:  \"))\n",
        "d = c*100\n",
        "print(a, b, c)\n",
        "print('결과값 =',d,'원 입니다')\n",
        "\n",
        "\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "lyJJl_hZDsUC",
        "outputId": "2884c8a1-16af-4293-982c-c0447fc13eb7"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "이름입력:  이우진\n",
            "전화번호입력:  01037401443\n",
            "택배g입력:  10\n",
            "이우진 01037401443 10\n",
            "결과값 = 1000 원 입니다\n"
          ]
        }
      ]
    }
  ]
}