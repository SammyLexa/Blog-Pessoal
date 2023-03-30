package org.generation.grafeat.model;

import java.math.BigDecimal;

import javax.persistence.Entity;
import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Id;
import javax.persistence.ManyToOne;
import javax.persistence.Table;
import javax.validation.constraints.NotBlank;
import javax.validation.constraints.NotNull;
import javax.validation.constraints.Size;

import com.fasterxml.jackson.annotation.JsonIgnoreProperties;

@Entity
@Table(name = "tb_produtos")

public class Produto {

	@Id
	@GeneratedValue(strategy = GenerationType.IDENTITY)
	private Long id;

	@NotBlank(message = "O nome do produto não pode ser vazio")
	@Size(min = 3, max = 100, message = "O nome deve conter no mínimo 3 e no máximo 100 caracteres.")
	private String nome;

	@NotBlank(message = "A descrição do produto não pode ser vazio")
	@Size(min = 3, max = 1000, message = "A descrição deve conter no mínimo 3 e no máximo 1000 caracteres.")
	private String descricao;

	@NotNull(message = "O preço do produto não pode ser vazio")
	private BigDecimal preco;

	private String material;

	@NotBlank(message = "O tamanho do produto não pode ser vazio")
	@Size(min = 3, max = 100, message = "O tamanho deve conter no mínimo 3 e no máximo 100 caracteres.")
	private String tamanho;

	@NotNull(message = "A quantidade do produto não pode ser vazia")
	private Long quantidade;

	@NotBlank(message = "A foto do produto não pode ser vazia")
	@Size(min = 3, max = 250, message = "O link deve conter no mínimo 3 e no máximo 250 caracteres")
	private String linkFoto;
	
	@ManyToOne
	@JsonIgnoreProperties("produto")
	private Categoria categoria;

	public Long getId() {
		return id;
	}

	public void setId(Long id) {
		this.id = id;
	}

	public String getNome() {
		return nome;
	}

	public void setNome(String nome) {
		this.nome = nome;
	}

	public String getDescricao() {
		return descricao;
	}

	public void setDescricao(String descricao) {
		this.descricao = descricao;
	}

	public BigDecimal getPreco() {
		return preco;
	}

	public void setPreco(BigDecimal preco) {
		this.preco = preco;
	}

	public String getMaterial() {
		return material;
	}

	public void setMaterial(String material) {
		this.material = material;
	}

	public String getTamanho() {
		return tamanho;
	}

	public void setTamanho(String tamanho) {
		this.tamanho = tamanho;
	}

	public Long getQuantidade() {
		return quantidade;
	}

	public void setQuantidade(Long quantidade) {
		this.quantidade = quantidade;
	}

	public String getLinkFoto() {
		return linkFoto;
	}

	public void setLinkFoto(String linkFoto) {
		this.linkFoto = linkFoto;
	}

	public Categoria getCategoria() {
		return categoria;
	}

	public void setCategoria(Categoria categoria) {
		this.categoria = categoria;
	}

}
